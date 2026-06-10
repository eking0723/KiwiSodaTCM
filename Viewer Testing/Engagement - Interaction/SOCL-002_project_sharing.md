## **SOCL-002:** Project Sharing  

> **Summary:** Verify that users can share project links via the browser share dialog or clipboard.  <br>

**Preconditions:** 
- User is on the project feed or a specific project details page.

Scenario 1: Sharing a project link

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Share2` (Share) button on a project card or details page | Verify that the button is visible. | 
 |  2 | Click the `Share` button | Verify that the system share dialog appears (if supported) OR the text "Copied!" appears on the button. | 
 |  3 | If clipboard was used, paste the link into a new tab | Verify that the pasted URL correctly points to the project (e.g., `/viewer/projects/[id]`). | 

**Post-conditions:**  
 - The project URL is successfully copied to the clipboard or shared via system tools.
 - The button provides visual feedback ("Copied!") after a successful copy.

