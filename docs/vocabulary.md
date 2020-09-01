*Please consult [Contact Details](contact.md) for the latest specific contact information.*

# Viva IT Vocabulary

We try and make sure that we use language that isn't too full of technical jargon where it can be avoided. We generally don't want to use abbreviations a lot (especially with newcomers). However like most other companies and organisations in the world, Viva IT has a vocabulary that's developed internally to refer to our products, processes, tools and techniques.

## Acceptance Criteria (AC)
> https://en.wikipedia.org/wiki/Acceptance_testing

The AC helps define what a task should do, consider it a minimum to the task being signed off by the ultimate client. It may be changed over time (this will be considered a scope extension and may attract a re-estimate), it may be reduced, it may be 'spun-out' into another task. The user-acceptance criteria may be defined by this (what will be tested in UAT)

## Apollo

The name for our suite of joined-up services, from the form a member completes on their app through to the automated decisioning and import into your back office software, and everything in between.

## Apollo Flow (APF)
> https://github.com/vivait/apollo-flow 

Apollo Flow - Data capture platform with workflows

## Apollo Launchpad (APL)

Our current credit union workstream management tool which will replace Task Stack in the long term.

## Apollo Web (APW)
> https://github.com/vivait/apollo-web

The web application for Apollo

## Apollo Mobile (AMO)
> https://github.com/vivait/apollo-mobile

The native mobile application for Apollo which is available for IOS and Android devices.

## Apollo NXG (APP)
> https://github.com/vivait/apollo-nxg

Next-generation data platform for credit unions. The software that provides the core logic and functionality of the Apollo services. 

## Airlock

Our business continuity service which allows member queries to be handled remotely from balance enquiries to filling in forms, even during times where you experience server issues.

## Backlog

The total of your work items and requests, tagged by priority. Our development 'todo list' for you.

## Credit Union (CU)
> A credit union is a member-owned financial cooperative, controlled by its members and operated on the principle of people helping people, providing its members credit at competitive rates as well as other financial services. https://en.wikipedia.org/wiki/Credit_union

## Helpdesk

Our developer-monitored helpdesk and the second port of call for your staff for all helpdesk issues or bugs.

## Infinity

The programme most of our partners are on which provides full access to our services, and time each month to spend on development and customisation.

## Launchpad

Our new credit union workstream management tool with more powerful automations and advanced logic. Notably includes everything TaskStack did plus functionality for openbanking, esigning, decisioning and much more.

## LinkedIn User Group

A community space for our partners to share tips and best practices, and get involved with out latest R&D developments and features. Talk you your account manager for access.

## Planning Poker (PP)

Planning poker, this is a method for roughly estimating the requirements (time and resources) of work, more details can be found in [Scrum and PP](scrum.md) 

## Rabbit Hole

An internal development term to imply that once you are in the rabbit hole you cannot extract yourself without significant effort, often not towards the overall goal. Rabbit holes should be approached with extrieme caution as they can be a whole waste of time and a source of frustration. It is useful to identify rabbit holes early so you can seek out senior help at the earliest possible time and thus tagging the issue `Complex`

## Scorecard

Creates a score based on heavily customisable factors, usually for a specific form. Can be used to intelligently route the flow of your forms and processes automatically.  One example might be sending out a different message depending on the time of day a form is received to manage customer expectations, another might be calculating whether a credit search must be performed on a loan application of a certain value.

## Status Page

Our main system status update and outage reporting site. The first port of call for your staff for all helpdesk issues or bugs.

## Task Types

**Deliverable:** A deliverable is a unit of development that groups up individual tasks into an overall deliverable, for example, "Automatic Credit Searching" may be a deliverable which will encompass multiple tasks to achieve this deliverable. Generally speaking a deliverable can be user-acceptance-tested, however the individual tasks are more likely to be tested individually.

**Task:** A task can be seen as a unit of development that can be operated on independently. It might be possible that two or more developers can pick up tasks within the same deliverable and be able to work collaboratively without 'stepping on toes'. Once a task has been developed, it can be user-acceptance-tested by the client. An example Task might be 'Migration of Database from Schema A to Schema B' to support the deliverable.

**Subtask:** A task that is further broken down into a unit of development that does not need user-acceptance-tested, and could serve as a 'todo' list for a larger Task. It would still have to be tested, but the client typically does not need to know about subtasks and they may contain development heavy terminology.

It is not necessary to have all task types, for efficiency and brevity only split up deliverables and tasks if there is a practical need.

## TaskStack

Our original credit union workstream management tool, currently being phased out.

## Timebox
A timebox is when an amount of time is placed onto a task instead of an estimate if the scope of the task is unknown/unclear. Once the time limit that was set has been reached, progress through the task will be assessed and the next step will be determined. The next step is usually just an extension of the timebox (causing the process to repeat) or a formal planning poker session.

Timeboxes are useful for proof-of-concepts and investigation into third-party services/systems.

## Tracking Code

Issued via the Helpdesk or youtrack, a code similar to 'ABC-123' unique for tracking the status of each work item with us. A 'case reference'.

## Upsource

The code review software used by the Viva IT team to manage and coordinate the work items we are undertaking for you (both new development and helpdesk tickets).

## User Acceptance Testing (UAT)

The end-user version of AC.

## Workflow Specification

The spreadsheets we create to provide instructions to our development team on how to construct your forms.

## Work In Progress (WIP)

Abbreviation used in Git Commits to indicate the branch or code is not ready for merging.

## YouTrack

The issue tracking software used by the Viva IT team to manage and coordinate the work items we are undertaking for you (both new development and helpdesk tickets).

## Zombie Task

Slow moving tasks that don't get completed, or are at risk of not being completed. They can have a tendancy to consume a lot of time through client correspondence or internal discussions but they cannot be completed. This could be because they are poorly specified or they represent extremely long processes with multiple stages of completion, in this case they should be converted to deliverables with an Acceptance Criteria that can be tracked with milestones. They should be clearly identified with a `Zombie` tag in YouTrack.
