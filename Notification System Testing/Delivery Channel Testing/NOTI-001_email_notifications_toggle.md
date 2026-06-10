## **NOTI-001:** Email Notifications Toggle  

> **Summary:** Verify that disabling email alerts stops all automated VSU email notifications.  <br>

**Preconditions:** 
- User is logged in.
- User is on the `Settings` page.

Scenario 1: Disabling email notifications

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Email Notifications` toggle in the "Notification Delivery" section | Verify that the current state is reflected (Enabled/Disabled). | 
 |  2 | Click the toggle to switch it to the `Off` (gray) position | Verify that the toggle UI updates instantly. | 
 |  3 | Click the `Save Changes` button at the top | Verify that a "Saving preferences..." indicator appears and then "Saved!". | 
 |  4 | Observe the `profiles` table in the database | Verify that `email_alerts` is now set to `false`. | 

**Post-conditions:**  
 - The `NotificationDispatcher` will skip the email channel for this user in future dispatches.
 - No emails are sent via the `send-email-notification` Edge Function for this user.
