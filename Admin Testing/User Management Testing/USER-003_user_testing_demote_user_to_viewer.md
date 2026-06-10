## **USER-003:** User Testing - Demote User to Viewer  

> **Summary:** Verify that user is demoted as standard viewer.  <br>

**Preconditions:**
- Device must be connected to the internet
- At least one `Project Manager` user type exists in the system.
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: 12345678)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `User Management` on the navigation bar     | Verify that the user is redirected to the `User Management` page   | 
 |  3 |Enter "Marylle" on the `Search` bar on the right side of the page      | Verify that the user being searched appears on the user table   |
 |  4 |Click on the Kebab Menu (three vertical dots) at the `Actions` column to open action options      | Verify that the action options appear (Promote to PM, View Activity Logs, and Remove User)  | 
 |  5 |Click `Demote to Viewer` option      | Verify that a confirmation dialouge appears on the screen | 
 |  6 |Click `Confirm` button      | Verify that the `Confirm` button changed in to "processing" with loading animation   | 
 |  7 |Wait until the processing animation finishes | Verify that the role in the `Role` column has been updated to `Viewer` successfully|

**Post-conditions:**  

 - User role has been updated in the Supabase
