## **FEED-006:** Infinite Scroll Performance  

> **Summary:** Verify that the project feed loads more content as the user scrolls down.  <br>

**Preconditions:** 
- Total number of projects exceeds the initial limit (usually 5-10 projects).
- User is on the landing page or viewer dashboard.

Scenario 1: Scrolling through the project feed

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Scroll to the bottom of the first set of projects in the feed | Verify that a `Loader2` (spinner) appears briefly at the bottom of the grid. | 
 |  2 | Maintain scroll position at the bottom | Verify that `fetchNextPage` is triggered and new projects are appended to the list. | 
 |  3 | Continue scrolling until all projects are loaded | Verify that the loader stops appearing when `hasNextPage` is false. | 
 |  4 | Observe the message at the bottom of the feed | Verify that the message "You've reached the end of the feed." appears. | 

**Post-conditions:**  
 - More projects are fetched and displayed without a full page reload.
 - Scroll position is maintained as new items are added.

