## **PJTT-003:** Task Creation & Assignment  

> **Summary:** Verify that Project Leads can create tasks and assign them to specific team members.  <br>

**Preconditions:** 
- User is logged in as Project Lead.
- Team members are already added to the project.

Scenario 1: Creating and assigning a task

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `Assign Task` button in the `Tasks & Team` tab | Verify that the "Assign New Task" dialog appears. | 
 |  2 | Enter a `Task Title` (e.g., "Draft Event Program") | Verify that the title is accepted. | 
 |  3 | Select a member from the `Assign To` dropdown | Verify that the list contains all currently assigned project members. | 
 |  4 | Select a `Due Date` | Verify that the date picker defaults to today or future dates. | 
 |  5 | Click `Create Task` | Verify that a loading spinner appears and the dialog closes on success. | 
 |  6 | Observe the `Task management` list | Verify that the new task is displayed with the correct assignee and due date. | 

**Post-conditions:**  
 - A new entry is added to the `tasks` table.
 - The assigned member receives a notification with a link to the task.

