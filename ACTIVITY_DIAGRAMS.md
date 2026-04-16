
Activity Workflow Modeling
1. User Registration
flowchart TD
Start --> EnterDetails
EnterDetails --> Validate
Validate -->|Valid| CreateAccount
Validate -->|Invalid| Error
CreateAccount --> End
Error --> End
Explanation

This workflow shows how a user registers. It ensures only valid data is accepted.

2. Login Process
flowchart TD
Start --> EnterLogin
EnterLogin --> CheckDetails
CheckDetails -->|Valid| AccessSystem
CheckDetails -->|Invalid| ShowError
AccessSystem --> End
ShowError --> End
3. Create Task
flowchart TD
Start --> OpenForm
OpenForm --> EnterTask
EnterTask --> SaveTask
SaveTask --> End
4. Edit Task
flowchart TD
Start --> SelectTask
SelectTask --> EditDetails
EditDetails --> SaveChanges
SaveChanges --> End
5. Delete Task
flowchart TD
Start --> SelectTask
SelectTask --> ConfirmDelete
ConfirmDelete --> DeleteTask
DeleteTask --> End
6. Set Deadline
flowchart TD
Start --> SelectTask
SelectTask --> SetDate
SetDate --> SaveDeadline
SaveDeadline --> End
7. Mark Task Complete
flowchart TD
Start --> SelectTask
SelectTask --> MarkComplete
MarkComplete --> End
8. Send Reminder
flowchart TD
Start --> CheckDeadline
CheckDeadline -->|Time reached| SendNotification
SendNotification --> End
Explanation

These workflows show how users interact with the system step by step.
They match your use cases and ensure the system works correctly.