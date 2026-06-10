## **PMPG-002:** Projects Sorting - Alphabetic & Date  

> **Summary:** Verify sorting: Newest First, Oldest, A-Z, and Z-A.  <br>

**Preconditions:** 
- User must be connected to internet.
- User must be logged in as Project Manager.  

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Project Manager` using these credentials: (email: 22-1-00856@vsu.edu.ph ; password: 12345678)   | Verify that the user is successfully logged in as Project Manager |  
 |  2 |Navigate to `Projects` page      | Verify that the user is redirected to the  `Projects` page |
 |  3 |Click on the `Filter` button beside the search bar      | Verify that a modal appears in the screen | 
 |  4 |Select `Newest First` option   | Verify that the project that appears in the project area is sorted in newest to oldest order of date created  | 
 |  5 |Select `Oldest First` option   | Verify that the project that appears in the project area is sorted in oldest to newest order of date created  | 
 |  6 |Select `Tiltle(A-Z)` option   | Verify that the project that appears in the project area is sorted in ascending alphabetical order of date created  |
 |  7 |Select `Tiltle(Z-A)` option   | Verify that the project that appears in the project area is sorted in descending alphabetical order of date created  |

**Post-conditions:**  

 - Shows the rendered UI for the request.
 - No specific changes in the database.  
