## **PMPG-003:** Projects Time Filter  

> **Summary:** Verify filters for 'All Time' (default) and 'This Month'.  <br>

**Preconditions:** 
- User must be connected to internet.
- User must be logged in as Project Manager.  

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Project Manager` using these credentials: (email: 22-1-00856@vsu.edu.ph ; password: 12345678)   | Verify that the user is successfully logged in as Project Manager |  
 |  2 |Navigate to `Projects` page      | Verify that the user is redirected to the  `Projects` page |
 |  3 |Click on the `Filter` button beside the search bar      | Verify that a modal appears in the screen |
 |  4 |Select `All Time` option   | Verify that all projects would appear in the project area| 
 |  5 |Select `This Month` option   | Verify that all project that was created during this month would appear in the project area| 

**Post-conditions:**  

 - Shows the rendered UI for the request.
 - No specific changes in the database.  
