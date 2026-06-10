## **CMT-002:** Comment Editing  

> **Summary:** Verify that users can edit their own comments.  <br>

**Preconditions:** 
- User is logged in as the author of an existing comment.
- User is on the project details page where the comment was posted.

Scenario 1: Editing an existing comment

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate your own comment in the `Student Feedback` list | Verify that an `Edit` (Pencil) button is visible on the comment. | 
 |  2 | Click the `Edit` button | Verify that the comment text is replaced by a textarea containing the current content. | 
 |  3 | Modify the comment text | Verify that the `Save` button is enabled. | 
 |  4 | Click the `Save` button | Verify that the textarea is replaced by the updated text and a loading state ("Saving...") is shown briefly. | 

Scenario 2: Attempting to edit another user's comment

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate a comment posted by a different user | Verify that the `Edit` (Pencil) button is NOT visible. | 

**Post-conditions:**  
 - The `content` column in the `comments` table is updated for the specific `comment_id`.
 - `updated_at` timestamp is refreshed in the database.

