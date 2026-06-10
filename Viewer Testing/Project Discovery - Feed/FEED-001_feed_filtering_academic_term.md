## **FEED-001:** Feed Filtering - Academic Term  

> **Summary:** Verify filtering projects by specific school years/terms.  <br>

**Preconditions:** 
- At least two different academic terms exist in the database (e.g., SY 2025-2026, SY 2024-2025).
- Projects are associated with different terms.

Scenario 1: Selecting a specific term from the Hero Banner

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the website OnTrack | Verify that the landing page displays the `HeroBanner` with a term selection dropdown. | 
 |  2 | Click the term selection dropdown (default is usually the current active term) | Verify that all available academic terms are listed in the dropdown. | 
 |  3 | Select a previous academic term (e.g., SY 2024-2025) | Verify that the URL search parameters update (e.g., `?term=UUID`). | 
 |  4 | Observe the project feed below | Verify that the `InfiniteProjectFeed` updates to show only projects belonging to the selected term. | 
 |  5 | Verify the term name in the Hero Banner | Verify that the Hero Banner background or title reflects the selected term's context. | 

**Post-conditions:**  
 - The project feed is filtered by the selected `term_id`.
 - The UI state persists the selected term in the URL.
