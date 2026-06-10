## **SOCL-001:** Follow Project Interaction  

> **Summary:** Verify following a project adds it to the user's following feed.  <br>

**Preconditions:** 
- User is logged in as `Viewer`.
- User is on the project feed or a specific project details page.

Scenario 1: Following a project

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Plus` (Follow) button on a project card (top right of the image) | Verify that the button is visible and indicates the project is not yet followed. | 
 |  2 | Click the `Plus` button | Verify that the icon changes to a `Check` or indicates "Following" status. | 
 |  3 | Navigate to the `Following` tab in the dashboard sidebar | Verify that the followed project now appears in the "Following" feed. | 
 |  4 | Observe the Follow button again | Verify that clicking it again (unfollowing) removes the project from the "Following" list. | 

**Post-conditions:**  
 - User's following status is updated in the `follows` table in the database.
 - The UI reflects the following status in real-time across the platform.
