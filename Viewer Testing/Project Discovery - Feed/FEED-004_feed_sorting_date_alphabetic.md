## **FEED-004:** Feed Sorting - Date & Alphabetic  

> **Summary:** Verify sorting projects by Newest, Oldest, and A-Z / Z-A titles.  <br>

**Preconditions:** 
- User is on the landing page or viewer dashboard.
- Multiple projects exist with different titles and creation dates.

Scenario 1: Applying different sorting options

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the `SlidersHorizontal` (filter) button next to the search bar | Verify that the dropdown menu shows "Sort By Date" and "Sort Alphabetically" sections. | 
 |  2 | Select `Oldest First` | Verify that the projects are reordered such that the earliest created project is at the top. URL should have `?sort=oldest`. | 
 |  3 | Select `Title (A to Z)` from the dropdown | Verify that projects are reordered alphabetically by their titles. URL should have `?sort=a-z`. | 
 |  4 | Select `Title (Z to A)` from the dropdown | Verify that projects are reordered in reverse alphabetical order. | 
 |  5 | Select `Newest First` (Default) | Verify that the most recently created project returns to the top. | 

**Post-conditions:**  
 - Project feed order updates dynamically based on the selected `sort` parameter.
 - The active sorting option is highlighted in the dropdown with a checkmark.

