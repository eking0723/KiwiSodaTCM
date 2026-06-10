## **FEED-005:** Feed Search - Live Debounce  

> **Summary:** Verify title/keyword search with live UI updates.  <br>

**Preconditions:** 
- User is on the landing page or viewer dashboard.
- Known project titles or keywords exist in the system.

Scenario 1: Searching for a specific project

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Type a keyword (e.g., "Nature") into the search input "Search projects by title or keywords..." | Verify that the text appears in the input field. | 
 |  2 | Wait for approximately 300ms without pressing Enter | Verify that a `Loader2` (spinner) briefly appears on the right side of the input field. | 
 |  3 | Observe the project feed | Verify that the feed automatically refreshes to show projects matching "Nature" in the title or description. | 
 |  4 | Observe the URL | Verify that `?q=Nature` is added to the URL parameters. | 
 |  5 | Clear the search input | Verify that the spinner appears again and the feed returns to its original state (all projects). | 

**Post-conditions:**  
 - Search results are fetched automatically after the debounce period.
 - The search query persists in the URL and remains active across status/sort changes.
