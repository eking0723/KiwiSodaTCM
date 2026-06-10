## **PJOV-003:** Project Deletion  

> **Summary:** Verify that Project Managers can permanently delete their projects and all associated data.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- Project exists and has associated tasks, milestones, and documents.

Scenario 1: Deleting a project

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Delete` (Trash2) button in the Project Header | Verify that the button is red and styled appropriately. | 
 |  2 | Click the `Delete` button | Verify that the `DeleteConfirmModal` appears asking to type the project name or confirm. | 
 |  3 | Click `Yes, Delete Task` (or the confirm button in the modal) | Verify that a loading spinner appears and the user is redirected to the `/project-manager` list page. | 
 |  4 | Observe the project list | Verify that the deleted project is no longer visible. | 

**Post-conditions:**  
 - Records are removed from `projects`, `tasks`, `project_milestones`, `project_documents`, and `budget_logs` tables.
 - Project-related files are removed from storage buckets.
 - A `PROJECT_DELETED` entry is added to the system activity logs.

