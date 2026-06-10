## **PJFB-001:** Feedback Monitoring  

> **Summary:** Verify that PMs can monitor all conversations and feedback counts.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- Project has existing student feedback.

Scenario 1: Monitoring feedback

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Navigate to the `Feedback` tab | Verify that the page header shows "Student Feedback" with description. | 
 |  2 | Observe the `Total Conversations` count | Verify it correctly reflects the number of top-level comments and replies. | 
 |  3 | Scroll through the conversation list | Verify that comments are sorted by date (newest first). | 
 |  4 | Observe comment metadata | Verify that user names, avatars, and "time ago" timestamps are visible. | 

**Post-conditions:**  
 - The UI accurately represents the data from the `comments` table.
 - Feedback count remains consistent with the database.

