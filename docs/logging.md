# Logging Guidelines

When developing software it is essential to have the right balance of logged events to develop and maintain the software
in the years to come. Log messages or event sent at the wrong level will quickly overwhelm the monitoring whereas events
that are not tracked or are too brief will need extensive code debugging to investigate an issue.

# Log Formatting 

When writing logs it is key to understand why they are used, if you need further context around a reported issue, you 
will be using the logs to get that. So some guidelines are:

* Try not to over capitalise:
 `Received Request to Import` should be `Received request to import` 
* Reference entity identifiers and enclose them in square brackets: `to import withdrawal` should be `to import Withdrawal [1]`
* When available use database ID's as entity identifiers
* When referencing variables, enclose them in single quotes: `for amount 1.00` should be `for amount '1.00'`
* Avoid calling ID's: `Withdrawal ID: [1]` should be `Withdrawal [1]` 
* Entity names should be capitalised: `to import withdrawal` should be `to import Withdrawal`

An example of "bad" log entries are:

```
 app.INFO: Received request to import withdrawal.
 app.INFO: Withdrawal successfully imported.
app.ERROR: Received 400 when trying to update ApplyingMember status for '11111111-1111-1111-1111-111111111111'
```

While writing code you can use the above to verify the execution path, however in production, when there are hundreds
of thousands of different entities flying around at different times to different services, the above will not give you 
much insight during an investigation.

Log entries such as the ones below allow you to glean much more insight into the workings of multiple systems working 
together without having to resort to debugging code.

```
    app.DEBUG: Withdrawal [1] request received to import
     app.INFO: Withdrawal [1] passed WithdrawalCheck [11111111-1111-1111-1111-111111111111]
   app.NOTICE: Withdrawal [1] to member [11111111-1111-1111-1111-111111111111] for amount '1.00' has been successfully imported
  app.WARNING: Withdrawal [1] has been made on bank account '11111111' not stored in backoffice
    app.ERROR: Withdrawal [1] could not import, already exists in database under db.dbo.main.source '1'
 app.CRITICAL: Withdrawal [1] could not import, server returned '500' and response: '{{"errors":{"withdrawal":["Withdrawal [1] is corrupt."]}}}'
app.EMERGENCY: Withdrawal [1] could not import, database connection timed out'
```

## Context
Where possible, you should supply context to the log entry through the 'context' facility of the logger (such as Monolog), this helps to collect metrics and to perform further investigation if needed.

For example, when processing a job, it would be useful to see the ID of that job during each logging entry, but this would become quickly cumbersome if you were reporting the ID on each line. Using the context means that it becomes possible to view threads of events, and supply additional information without worry about presenting it in 'human readable formatting'. In Monolog, the context array can be used for this purpose.

https://github.com/Seldaek/monolog/blob/master/doc/01-usage.md#using-the-logging-context

```php
            $this->logger->error(
                "Job [{$jobId}] threw a terminal exception: " . $exception->getMessage(),
                [
                    'jobId' => $jobId,
                    'exception' => $exception->getMessage(),
                    'stackTrace' => $exception->getTrace()
                ]
            );
```



# Logging Levels 

| Level | Name | When to use |
|---|---|---|---|
| 0  | Emergency | Significant fault or breach of security that needs IMMEDIATE investigation |
| 1  | Alert     | Significant fault or breach of security that needs IMMEDIATE investigation |
| 2  | Critical  | A failure state that requires IMMEDIATE investigation, these can usually trigger HTTP 500 errors which can bubble up to the user, resulting in visible problems. |
| 3  | Error     | A failure state that REQUIRES investigation at some point, however execution doesn't halt. Doesn't have to be a code level failure, could just be a domain issue (e.g. two S1 accounts) |
| 4  | Warning   | Notable failure events but still normal execution continues - requires no immediate notification. However the quantity of these events are monitored and excessive number of warnings could result in a fault. |
| 5  | Notice    | Notable neutral or positive but entirely normal events where execution continues - requires no notifications |
| 6  | Info      | A 'production level' debug - typically used to supply context to other log events when investigating. |
| 7  | Debug     | Very verbose information used by developers that is ignored except for when explicitly debugging. | 

# Typical Examples of Use

## Critical
* Sync payloads couldn't process (will result in stale data)
* Pages don't load at all on the front-end
* Member cannot load forms

## Error
* A duplicate transaction in a sync payload - it's ignored and carries on but should be addressed
* HTTP 400 was returned when submitting information from one service to another

## Warning
* A member has FAILED to log on
* A member has been banned

## Notice
* A member SUCCEEDED login
* A member COMPLETED a form
* Withdrawal SUCCESSFULLY imported

## Info
* A member is being synced
* A product's availability/eligibility is being checked

## Debug
* When a method is entered
* The entirety of an object
* Mapping the execution path
