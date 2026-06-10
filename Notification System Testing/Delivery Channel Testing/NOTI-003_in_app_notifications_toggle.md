## **NOTI-003:** In-App Notifications Toggle  

> **Summary:** Verify that in-app bell notifications can be enabled or disabled for real-time alerts.  <br>

**Preconditions:** 
- User is on the `Settings` page.

Scenario 1: Toggling in-app alerts

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `In-App Notifications` toggle to the `Off` position | Verify that the toggle UI updates. | 
 |  2 | Click `Save Changes` | Verify that the preference is saved successfully. | 
 |  3 | Trigger an event that would normally send a notification (e.g., as another user, comment on this user's project) | Verify that the notification bell icon does NOT show a new alert for this event. | 
 |  4 | Observe the `notifications` table in the database | Verify that NO new entry was created for this user-id. | 

**Post-conditions:**  
 - The `NotificationDispatcher` skips the `in_app` channel for this user.
 - Real-time updates to the notification list are suppressed.
