## **PJOV-002:** Project Visibility Toggle  

> **Summary:** Verify that Project Managers can publish or unpublish projects for public view.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- Project is currently in `Draft` or `Live` state.

Scenario 1: Publishing a project

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Publish` (Globe) button in the Project Header | Verify that the button is visible. | 
 |  2 | Click the `Publish` button | Verify that a "Publish Project?" confirmation modal appears. | 
 |  3 | Click `Confirm` | Verify that the project status badge changes from `Draft` to `Live` (with a pulsing green indicator). | 
 |  4 | Observe the visibility banner in the `Overview` tab | Verify that the banner turns green and states "Project is Live". | 

Scenario 2: Unpublishing a project

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `Unpublish` button in the Project Header | Verify that the "Unpublish Project?" modal appears. | 
 |  2 | Click `Confirm` | Verify that the status badge returns to `Draft`. | 

**Post-conditions:**  
 - The `live_status` column in the `projects` table is toggled between 'Draft' and 'Live'.
 - Live projects appear in the student project feed.

