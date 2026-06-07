## **ACTL-002:** Activity Log Testing - Search Log with Filter  

> **Summary:** Verify that user was able to search log/s using filter successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: password8086)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Content Moderation` on the navigation bar     | Verify that the user is redirected to the `Content Moderation` page   | 
 |  3 |Click on the `Filter` module beside the serach bar      | Verify that a dropdown menu appears   | 
 |  4 |Select `User Removal` option      | Verify that all of logs containing "User Deleted" appears in the table    |  

**Post-conditions:**  

- No changes in the database.
