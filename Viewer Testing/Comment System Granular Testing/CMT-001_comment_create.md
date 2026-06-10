## **CMT-001:** Comment Creation  

> **Summary:** Verify that authenticated users can post feedback on projects.  <br>

**Preconditions:** 
- User is logged in as `Viewer` or `Project Manager`.
- User is on a project's details page within the "Feedback" section.

Scenario 1: Posting a new comment

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Scroll to the `Student Feedback` section of a project | Verify that a textarea with placeholder "Share your thoughts or feedback..." is visible. | 
 |  2 | Enter a valid comment text | Verify that the `Post Feedback` button becomes enabled. | 
 |  3 | Click the `Post Feedback` button | Verify that a loading spinner appears on the button and the textarea is cleared after success. | 
 |  4 | Observe the comment list below | Verify that the new comment appears at the top of the list with the user's name and current time. | 

Scenario 2: Guest attempt to comment

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Navigate to a project details page as a `Guest` (not logged in) | Verify that the feedback section shows "Please login to leave feedback or reply". | 
 |  2 | Click the login prompt | Verify that the user is redirected to the `/login` page. | 

**Post-conditions:**  
 - Comment is saved in the `comments` table with correct `project_id` and `user_id`.
 - Feedback count for the project increments.

