## **PJOV-001:** Project Details Update  

> **Summary:** Verify that Project Managers can update basic project information (Title, Location, Description).  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- User is on the `Overview` tab.

Scenario 1: Updating Project Description

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Project Description` section and click the `Edit` (Pencil) icon | Verify that the "Edit Project Description" dialog appears. | 
 |  2 | Modify the description text in the textarea | Verify that the text can be edited and holds multiple lines. | 
 |  3 | Click `Save Description` | Verify that a loading spinner appears and the dialog closes on success. | 
 |  4 | Observe the `Overview` tab | Verify that the description section displays the updated text immediately. | 

Scenario 2: Updating Title and Location (via Header)

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | In the Project Header, click the `Edit` icon next to the title | Verify that the "Edit Project Details" dialog appears. | 
 |  2 | Change the `Project Title` and `Location` | Verify that the fields accept new values. | 
 |  3 | Click `Save Changes` | Verify that the header title and location metadata are updated. | 

**Post-conditions:**  
 - The `projects` table is updated with the new values.
 - `updated_at` timestamp is refreshed.

