## **NOTI-002:** Push Notifications Toggle  

> **Summary:** Verify that registering/unregistering for browser/mobile push alerts works correctly.  <br>

**Preconditions:** 
- Browser supports Web Push API.
- User is on the `Settings` page.

Scenario 1: Enabling push notifications

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `OS Push Notifications` toggle to the `On` position | Verify that a "Enabling push notifications..." toast appears. | 
 |  2 | Observe the browser permission prompt | Verify that the browser asks for notification permission. | 
 |  3 | Click `Allow` on the browser prompt | Verify that the toast updates to "Push notifications enabled". | 
 |  4 | Observe the `push_alerts` value in the database | Verify it is set to `true`. | 

Scenario 2: Disabling push notifications

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the toggle to the `Off` position | Verify that a "Disabling push notifications..." toast appears. | 
 |  2 | Observe the success message | Verify that the toggle turns gray and "Push notifications disabled" toast appears. | 

**Post-conditions:**  
 - Push subscription is managed via the `usePushNotifications` hook.
 - The `NotificationDispatcher` will include/exclude the push channel based on this setting.
