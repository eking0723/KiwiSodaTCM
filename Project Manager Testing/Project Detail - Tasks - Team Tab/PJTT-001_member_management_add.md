## **PJTT-001:** Member Management - Add  

> **Summary:** Verify that the Project Lead can add new members (Officers) to the project team.  <br>

**Preconditions:** 
- User is logged in as Project Manager (Project Lead).
- User is on the `Tasks & Team` tab.
- At least one Officer exists in the system who is not already a member of this project.

Scenario 1: Adding a new team member

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Scroll to the `Team Members` section and click `Add Member` | Verify that the "Add Officer to Project" dialog appears. | 
 |  2 | Click the `Select Officer` dropdown | Verify that only Officers NOT currently in the project are listed. | 
 |  3 | Select an Officer from the list | Verify that the `Add to Project` button becomes enabled. | 
 |  4 | Click `Add to Project` | Verify that a loading spinner appears and the dialog closes on success. | 
 |  5 | Observe the `Team Members` list | Verify that the new member is added with their name, role, and a "0/0 completed" task stat. | 

**Post-conditions:**  
 - A new entry is added to the `project_members` table.
 - The added Officer receives an in-app notification.
 - The UI updates in real-time.

