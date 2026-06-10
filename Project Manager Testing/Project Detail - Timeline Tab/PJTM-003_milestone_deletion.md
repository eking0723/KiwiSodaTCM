## **PJTM-003:** Milestone Deletion  

> **Summary:** Verify that Project Managers can permanently remove milestones.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- At least one milestone exists.

Scenario 1: Deleting a milestone

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Hover over a milestone and click the `Delete` (Trash2) icon | Verify that a "Delete Milestone?" confirmation dialog appears. | 
 |  2 | Observe the milestone title in the dialog | Verify it correctly identifies the milestone being deleted. | 
 |  3 | Click `Delete` in the dialog | Verify that the milestone is immediately removed from the UI and a success toast appears. | 
 |  4 | Click `Cancel` on a different milestone deletion attempt | Verify that the milestone remains in the list. | 

**Post-conditions:**  
 - The milestone record is removed from the `project_milestones` table.
 - This action is irreversible.

