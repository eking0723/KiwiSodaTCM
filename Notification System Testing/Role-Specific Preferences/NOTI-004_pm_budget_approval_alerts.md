## **NOTI-004:** PM: Budget Approval Alerts  

> **Summary:** Verify PM receives alerts for team member budget requests when enabled.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- User is on the `Settings` page.

Scenario 1: Toggling budget alerts

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Project Management Preferences` section | Verify that `Budget Approval Alerts` toggle is visible. | 
 |  2 | Click the toggle to enable/disable the preference | Verify the UI reflects the change. | 
 |  3 | Click `Save Changes` | Verify the preference is saved in the `profiles` table under `budget_alerts`. | 

**Post-conditions:**  
 - The `NotificationDispatcher` checks `budget_alerts` preference before sending relevant notifications.
