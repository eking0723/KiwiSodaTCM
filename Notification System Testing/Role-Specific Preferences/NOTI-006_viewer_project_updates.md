## **NOTI-006:** Viewer: Followed Project Updates  

> **Summary:** Verify Viewers receive alerts when projects they follow have updates.  <br>

**Preconditions:** 
- User is logged in as Viewer.
- User follows at least one project.

Scenario 1: Toggling project updates

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Viewer Preferences` section in Settings | Verify that `Followed Project Updates` toggle is visible. | 
 |  2 | Toggle the setting and click `Save Changes` | Verify it is saved in `followed_project_updates` column. | 
 |  3 | As a PM, update a milestone in a project this viewer follows | Verify that the viewer receives a notification ONLY if the preference was enabled. | 

**Post-conditions:**  
 - Notification routing depends on the `followed_project_updates` flag.

