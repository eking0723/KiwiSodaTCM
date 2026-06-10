## **PJFB-002:** Reply to Feedback  

> **Summary:** Verify that Project Managers can reply to student feedback on their projects.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- At least one student comment exists in the `Feedback` tab.

Scenario 1: Replying to a student comment

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Navigate to the `Feedback` tab of a project | Verify that the comment list is displayed. | 
 |  2 | Locate a student comment and click `Reply` | Verify that a "Write a reply..." textarea appears below the comment. | 
 |  3 | Enter a professional response (e.g., "Thank you for the suggestion!") | Verify that the text is accepted. | 
 |  4 | Click `Post Reply` | Verify that a loading state ("Posting...") appears and the reply is added to the thread. | 
 |  5 | Observe the indentation | Verify that the reply is indented relative to the parent comment. | 

**Post-conditions:**  
 - A new entry is added to the `comments` table with the correct `parent_id`.
 - The student who posted the original comment receives a notification.
 - The UI updates in real-time.

