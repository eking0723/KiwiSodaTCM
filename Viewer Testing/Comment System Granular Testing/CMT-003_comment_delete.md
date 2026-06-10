## **CMT-003:** Comment Deletion  

> **Summary:** Verify that users can delete their own comments.  <br>

**Preconditions:** 
- User is logged in as the author of an existing comment (or as a Project Manager/Admin).
- User is on the project details page where the comment was posted.

Scenario 1: Deleting a comment

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate a comment you have permission to delete | Verify that a `Delete` (Trash2) button is visible. | 
 |  2 | Click the `Delete` button | Verify that a browser confirmation dialog appears ("Are you sure you want to delete this comment?"). | 
 |  3 | Click `OK` (Confirm) | Verify that the comment is removed from the list immediately. | 
 |  4 | Click `Cancel` on the dialog | Verify that the comment remains in the list. | 

**Post-conditions:**  
 - The comment is removed from the `comments` table in the database.
 - If the comment had replies, their visibility/structure might be affected (depending on cascade settings, usually they are also deleted or orphaned).

