## **PJTT-002:** Member Management - Remove  

> **Summary:** Verify that project members can be removed from the team (Admin or Project Deletion context).  <br>

**Preconditions:** 
- User is logged in as Project Manager (Project Lead) or Admin.
- The project has at least one member assigned.

Scenario 1: Removing a member via Project Deletion (PM)

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | In the Project Manage Header, click the `Delete` button | Verify that the "Delete Project?" confirmation modal appears. | 
 |  2 | Click `Confirm` to delete the project | Verify that the project and all its associations are removed. | 
 |  3 | Observe the `project_members` table in the database | Verify that all records associated with this `project_id` are deleted. | 

Scenario 2: Standalone Member Removal (Admin Context)

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | (As Admin) Navigate to User Management | Verify that users can be managed globally. | 
 |  2 | Locate the user to be removed and select "Delete User" | Verify that the system removes the user from ALL project teams they are part of. | 

**Post-conditions:**  
 - Member association is severed in the `project_members` table.
 - Note: Standalone individual member removal by PM is currently handled via project lifecycle management.

