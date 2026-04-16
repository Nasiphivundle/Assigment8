
Object State Modeling
1. Task Object State Diagram
stateDiagram-v2
[*] --> Created
Created --> InProgress : User starts task
InProgress --> Completed : Mark as complete
InProgress --> Overdue : Deadline passed
Overdue --> Completed : Task finished late
Completed --> [*]
Explanation

The Task object moves through different states such as Created, InProgress, Completed, and Overdue.
This relates to functional requirements like creating tasks, setting deadlines, and marking tasks as complete.

2. User Account State Diagram
stateDiagram-v2
[*] --> Registered
Registered --> Active : Login successful
Active --> Locked : Too many failed attempts
Locked --> Active : Admin unlocks account
Active --> LoggedOut : User logs out
LoggedOut --> Active : Login again
Explanation

The User Account changes from Registered to Active when logged in.
This supports login and security requirements.

3. Reminder State Diagram
stateDiagram-v2
[*] --> Scheduled
Scheduled --> Sent : Time reached
Sent --> Delivered : Notification received
Delivered --> [*]
Explanation

This shows how reminders are scheduled and sent to users.
It supports the requirement of sending reminders before deadlines.

4. Assignment Object State Diagram
stateDiagram-v2
[*] --> Created
Created --> Assigned : Lecturer assigns
Assigned --> InProgress : Student starts work
InProgress --> Submitted : Student submits
Submitted --> Reviewed : Lecturer reviews
Reviewed --> [*]
Explanation

This diagram shows how assignments move through stages.
It supports lecturer and student interactions.

5. System Task Status
stateDiagram-v2
[*] --> ToDo
ToDo --> InProgress : Start task
InProgress --> Testing : Development done
Testing --> Done : Passed test
Testing --> Blocked : Issues found
Blocked --> InProgress : Issue fixed
Done --> [*]
Explanation

This reflects your Kanban board workflow (Assignment 7).
It shows how tasks move from To Do to Done.
