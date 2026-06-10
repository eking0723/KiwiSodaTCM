## **PJTM-001:** Milestone Creation  

> **Summary:** Verify that Project Managers can add new milestones to the project timeline.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- User is on the `Timeline` tab of a specific project.

Scenario 1: Adding a new milestone

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `Add Milestone` button | Verify that the "Add New Milestone" dialog appears. | 
 |  2 | Enter a `Milestone Title` (e.g., "Logistics Planning") | Verify that the title is accepted. | 
 |  3 | Select a `Target End Date` | Verify that the date picker allows date selection. | 
 |  4 | Enter `Progress (%)` (default 0) | Verify that the value is within 0-100 range. | 
 |  5 | Select a `Status` (e.g., "Proposed") | Verify that the status options are available. | 
 |  6 | Click `Add Milestone` button in the dialog | Verify that a loading spinner appears and the dialog closes on success. | 
 |  7 | Observe the timeline list | Verify that the new milestone appears with its title, target date, and progress bar. | 

**Post-conditions:**  
 - A new entry is added to the `project_milestones` table.
 - The UI updates in real-time for all connected clients.

