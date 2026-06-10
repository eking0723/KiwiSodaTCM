## **FEED-002:** Feed Filtering - Status Tabs  

> **Summary:** Verify filtering projects by 'All', 'Ongoing', and 'Completed' statuses.  <br>

**Preconditions:** 
- User is on the landing page or viewer dashboard.
- Projects with both 'Ongoing' and 'Completed' statuses exist for the selected term.

Scenario 1: Switching between status tabs

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the status filter tabs (All, Ongoing, Completed) below the Project Dashboard title | Verify that the 'All' tab is selected by default and shows all projects. | 
 |  2 | Click the `Ongoing` tab | Verify that the project feed refreshes and only projects with progress < 100% are displayed. | 
 |  3 | Observe the URL and loader | Verify that `?status=ongoing` is added to the URL and a loader or "Updating results..." indicator briefly appears. | 
 |  4 | Click the `Completed` tab | Verify that only projects with 100% progress are displayed in the feed. | 
 |  5 | Click back to the `All` tab | Verify that the feed returns to showing both ongoing and completed projects. | 

**Post-conditions:**  
 - Projects are filtered based on their `status` or `progress` level.
 - Tab selection is reflected in the URL search parameters.

