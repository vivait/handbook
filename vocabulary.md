# Vocabulary

On the whole, we have a dislike for most buzzwords. So if you're looking for a place where _DYNAMIC SYNERGY_ during _CRUNCH TIME_ is how you _KNOCK IT OUT OF THE PARK, YO_, this likely isn't the place for you.

We try and make sure that we use language that isn't too full of technical jargon where it can be avoided. We generally don't want to use abbreviations a lot (especially with newcomers). However like most other companies and organisations in the world, Viva IT has a vocabulary that's developed internally to refer to our products, processes, tools and techniques.

## CU ([Credit Union](https://en.wikipedia.org/wiki/Credit_union))

>A credit union is a member-owned financial cooperative, controlled by its members and operated on the principle of people helping people, providing its members credit at competitive rates as well as other financial services.

## AC ([Acceptance Criteria](https://en.wikipedia.org/wiki/Acceptance_testing))

The AC helps define what a task should do, consider it a minimum to the task being signed off by the ultimate client. It may be changed over time (this will be considered a scope extension and may attract a re-estimate), it may be reduced, it may be 'spun-out' into another task. The user-acceptance criteria may be defined by this (what will be tested in UAT)

## UAT (User Acceptance Testing)

The end-user version of AC

## PP ([Planning Poker](https://en.wikipedia.org/wiki/Planning_poker))

While typically done in the fashion described [here](https://www.mountaingoatsoftware.com/agile/planning-poker) - ours is slightly different. We don't stick to set story points, because we use hours to estimate tasks. Therefore we each estimate how long a task will take, and keep our estimate secret until revealing it once everyone has one. Through this, we will then either discuss the times (if there's a wide variance in high & low time estimates) or generally pick the higher estimate if the estimates are all fairly similar. For example, if 2 people say 4 hours and one person says 5, we might discuss it and either could be valid. But if 2 people say 5 hours and one person says 4, we'll likely pick 5 hours.

## Task Types

**Deliverable:** A deliverable is a unit of development that groups up individual tasks into an overall deliverable, for example, "Automatic Credit Searching" may be a deliverable which will encompass multiple tasks to achieve this deliverable. Generally speaking a deliverable can be user-acceptance-tested, however the individual tasks are more likely to be tested individually.

**Task:** A task can be seen as a unit of development that can be operated on independently. It might be possible that two or more developers can pick up tasks within the same deliverable and be able to work collaboratively without 'stepping on toes'. Once a task has been developed, it can be user-acceptance-tested by the client. An example Task might be 'Migration of Database from Schema A to Schema B' to support the deliverable.

**Subtask:** A task that is further broken down into a unit of development that does not need user-acceptance-tested, and could serve as a 'todo' list for a larger Task. It would still have to be tested, but the client typically does not need to know about subtasks and they may contain development heavy terminology.

It is not necessary to have all task types, for efficiency and brevity only split up deliverables and tasks if there is a practical need.

