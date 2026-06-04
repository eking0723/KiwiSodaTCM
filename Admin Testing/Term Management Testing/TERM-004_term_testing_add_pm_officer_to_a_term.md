## **TERM-004:** Term Testing - Add PM/Officer to a Term  

> **Summary:** Verify that user was able to add project manager/officer to a term.  <br>

**Preconditions:** 
- Device must be connected to the internet
- At least a `Term` exists in the system.
- At least one `Project Manager` user type existed in the system.
- User must be logged in as `Admin` 
 
Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: password8086)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Term Management` on the navigation bar     | Verify that the user is redirected to the `Term Management` page   |
 |  3 |Click the Kebab Menu (vertical three dots) in the `Action` column     | Verify that a dropdown option appears   |
 |  4 |Click `Manage Term` option      | Verify that a Term management dialouge card appears   |
 |  5 |Select a user in the `Project Manager` dropdown field     | Verify that the selected user appears in the field   |
 |  6 |Set the Position to "President"      | Verify that the entry is saved in the input field   |  
 |  7 |Click `Add` button      | Verify that the user is successfully assigned to the term  |  

**Post-conditions:**  

 - The term `project-manager` with its corresponding `position` is saved Supabase.
 - The number of `Officers` automatically adjusts.
