# Info
A 'production level' debug - less verbose version of debug

• A member is being synced
• A product availability is bei

# Notice
Any positive state but normal execution continues - requires no immediate intervention (dev OR ops)

• A member SUCCEEDED login
• A member started a form

# Warning
Any failure state but normal execution continues - requires no immediate intervention (dev OR ops)

• A member has FAILED to log on
• A member has been banned

# Error
A failure state that REQUIRES investigation, but execution doesn't halt. Doesn't have to be a code level failure, could just be a domain issue (e.g. two S1 accounts)

• A duplicate transaction in a sync payload - it's ignored and carries on but should be addressed

# Critical
A failure state that requires IMMEDIATE/this-day investigation. This will impact service usage a lot.

• Sync payloads don't process at all
• Pages don't load at all on the front-end
• Member cannot load forms

# Emergency
Immediate showstopper - everyone notified
