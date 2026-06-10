## **PJTT-005:** Task Status Management  

> **Summary:** Verify task status updates and their impact on progress percentage.  <br>

**Preconditions:** 
- User is logged in as Project Lead.
- A task is currently in "Awaiting Review" status (submitted by a member).

Scenario 1: Approving a completed task

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate a task with the `Awaiting Review` (pulsing amber) badge | Verify that an `Approve` button is visible next to the badge. | 
 |  2 | Click the `Approve` button | Verify that the task status changes to `Completed` (green) and the `Approve` button disappears. | 
 |  3 | Observe the member stats below | Verify that the completion ratio (e.g., 1/2) and progress bar update for the assigned member. | 

Scenario 2: Handling overdue tasks

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate a task where the due date has passed | Verify that the status badge shows `Overdue` (red). | 
 |  2 | Click the `Force Complete` button (if visible for overdue tasks) | Verify that the task status is set to `Completed`. | 

**Post-conditions:**  
 - The `tasks` table is updated with the new `status`.
 - Project overall progress might be affected (if tied to task completion).
