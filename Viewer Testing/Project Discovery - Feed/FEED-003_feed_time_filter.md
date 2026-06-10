## **FEED-003:** Feed Filtering - Time  

> **Summary:** Verify filtering projects by 'All Time' and 'This Month'.  <br>

**Preconditions:** 
- User is on the landing page or viewer dashboard.
- At least one project was created this month, and some projects were created earlier.

Scenario 1: Filtering by time using the dropdown

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `SlidersHorizontal` (filter) button next to the search bar | Verify that a dropdown menu appears with "Filter By Time" section. | 
 |  2 | Select `This Month` | Verify that the URL updates with `?date=month`. | 
 |  3 | Observe the project feed | Verify that only projects created within the current calendar month are visible. | 
 |  4 | If no projects match, observe the UI | Verify that an empty state icon (Inbox) appears with the message "No projects this month". | 
 |  5 | Re-open the filter dropdown and select `All Time` | Verify that the filter is removed (`?date=all`) and all projects are shown again. | 

**Post-conditions:**  
 - Projects are filtered based on their `created_at` timestamp.
 - Empty state correctly reflects the active time filter.

