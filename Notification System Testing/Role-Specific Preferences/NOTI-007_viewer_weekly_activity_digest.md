## **NOTI-007:** Viewer: Weekly Activity Digest  

> **Summary:** Verify Viewers receive weekly summaries of USSC activities when enabled.  <br>

**Preconditions:** 
- User is logged in as Viewer.
- User is on the `Settings` page.

Scenario 1: Toggling weekly digest

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Weekly Activity Digest` toggle | Verify it is visible for Viewer role. | 
 |  2 | Toggle the setting and click `Save Changes` | Verify it is saved in `weekly_digest` column. | 
 |  3 | Observe system behavior | Verify that the background job for weekly digests filters recipients by this preference. | 

**Post-conditions:**  
 - Weekly email dispatches are managed based on this preference.

