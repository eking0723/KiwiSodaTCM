## **USER-005:** User Testing - Viewer User Logs  

> **Summary:** Verify that the system shows correct viewer logs.  <br>

**Preconditions:** 
- Device must be connected to the internet
- At least on other user exists in the system.
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: 12345678)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `User Management` on the navigation bar     | Verify that the user is redirected to the `User Management` page   | 
 |  3 |Enter "Marylle" on the `Search` bar on the right side of the page      | Verify that the user being searched appears on the user table   |
 |  4 |Click on the Kebab Menu (three vertical dots) at the `Actions` column to open action options      | Verify that the action options appear (Promote to PM, View Activity Logs, and Remove User)  | 
 |  5 |Click `View Activity Logs` option      | Verify that the user is redirected to `Activity Logs` page  | 
 |  6 |Observe the table      | Verify that the activity logs appear in order (latest logs at the top)   |  

**Post-conditions:**  

 - Review on the activity logs of a user 