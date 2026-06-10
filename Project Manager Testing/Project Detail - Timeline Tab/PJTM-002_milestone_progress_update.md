## **PJTM-002:** Milestone Progress Update  

> **Summary:** Verify that updating a milestone's progress and status reflects on the timeline.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- At least one milestone exists in the project.

Scenario 1: Updating an existing milestone

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Hover over a milestone in the `Timeline` list | Verify that the `Edit` (Pencil) icon becomes visible. | 
 |  2 | Click the `Edit` icon | Verify that the "Edit Milestone" dialog appears with current values. | 
 |  3 | Change the `Progress (%)` (e.g., to 100) and `Status` (e.g., to "Completed") | Verify that the inputs accept the changes. | 
 |  4 | Click `Save Changes` | Verify that the dialog closes and the milestone updates in the list. | 
 |  5 | Observe the milestone icon | Verify it changes to a `Check` icon (for Completed status). | 
 |  6 | Observe the progress bar | Verify it is now fully filled (100%). | 

**Post-conditions:**  
 - The `project_milestones` table is updated with new `progress` and `status` values.
 - Real-time synchronization ensures other managers see the update.

