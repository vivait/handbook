## Overview

The Viva IT team pride ourselves on the reliability of our services and how they make life easier for our clients and their customers. That is why we treat showstoppers very seriously. This page explains what they are and how we handle them.

A showstopper is defined as a hardware or software bug of extreme severity which requires an immediate fix. Prioritising an issue as a showstopper is a proactive and subjective judgement made by anyone in the team who becomes aware of an extremely urgent issue. Don't worry about raising a ‘false alarm’, as we would rather have false alarms than missed showstoppers.

## Summary - Temporary key showstopper roles

*Incident Leader* - The most experienced developer available. Leads efforts to diagnosis & fix. Usually updates status.vivait.co.uk

*Pair Programmer* - A developer who sits with Incident Leader and assists them and peer reviews work.

*Showstopper Developer* - A developer working on the showstopper at their own desk.

*Liaison Developer* - A developer who updates the Account Manager.

*Other Developers* - Developers who follow progress as they may be called in to get involved at any time.

*Account Manager* - The individual responsible for usual client contact. Fields questions from affected users and provides any updates to external parties that fall outside of the scope of [https://status.vivait.co.uk](https://status.vivait.co.uk).

## Showstopper Protocol

### Declaring a Showstopper

Declare a showstopper by changing the 'priority' of a YouTrack issue to 'Show-stopper'. This causes an automated notification to appear in the #service-status channel of the Viva IT Slack group. Once made aware of the issue in this way, team members should be ready to put what they are currently working on aside.

The most senior developer available in terms of experience takes ownership of the showstopper incident and leads the team, who instantly shift into a more hierarchical and controlled way of working than normal. 

### Team Formation

This ‘[Incident leader](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles)’ will soon nominate which developers are needed to directly assist them in diagnosis and fixing of the showstopper. It is also typical for a developer to sit with the [Incident leader](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) in a form of pair programming, due to the need for a faster code review process. Any developers involved in the showstopper will typically set their Slack status to very busy (a red heart icon) to communicate their involvement, and so that they are not interrupted or ‘context switched’ regarding less important manners.

### Communications

During the first few minutes of a showstopper the [Incident leader](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) will likely update the [https://status.vivait.co.uk](https://status.vivait.co.uk) page and instruct the [Account Manager](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) on any relevant initial communications to make.

As the [Incident leader](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) will not have the time to explain ongoing developments to the [Account Manager](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) in a suitable format, nor answer questions, a developer who is not required directly to fix the showstopper will act as [liaison](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) between [Incident leader](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) and [Account Manager](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) by listening in to the technical situation from the [Incident leaders](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) desk in a non-disruptive way, and then going away and talking to the [Account Manager](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) to translate the update into a less technical format and attempt to answer any questions. 

Any [other developers](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) will listen in and follow #service-status to observe the general situation as there is always a chance they will be needed to help. Internal correspondence during a showstopper incident should be logged clearly in #service-status, including summaries of key verbal conversations. A more explicit and clear level of detail in communications is required during showstopper incidents to effectively keep the team apprised and in unison on the status of a potentially fast moving and fluid situation.

### Etiquette

Team members involved in key roles are encouraged not to take take breaks during a showstopper incident until afterwards. As we have not yet experienced a showstopper of a long duration this has never (yet) been an issue. In a (theoretical) extended duration showstopper a clear handoff to another team member would be required. 

### Closure

The [Incident leader](https://github.com/vivait/handbook/blob/master/showstopper.md#summary---temporary-key-showstopper-roles) (only) will declare when the showstopper incident is over, and update [https://status.vivait.co.uk](https://status.vivait.co.uk). They will also declare what follow-up works or monitoring will take place. At this point the showstopper roles are abandoned and normal work resumed, however often a retrospective will be scheduled in the near future to analyse the incident (root causes, improvements).
