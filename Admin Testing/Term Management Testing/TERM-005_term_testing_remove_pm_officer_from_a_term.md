## **TERM-005:** Term Testing - Remove PM/Officer from a Term  

> **Summary:** Verify that user was able to remove project manager/officer to a term.  <br>

**Preconditions:** 
- Device must be connected to the internet
- At least a `Term` exists in the system.
- An officer/project manager exixts in the term.
- User must be logged in as `Admin` 
 
Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: password8086)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Term Management` on the navigation bar     | Verify that the user is redirected to the `Term Management` page   |
 |  3 |Click the Kebab Menu (vertical three dots) in the `Action` column     | Verify that a dropdown option appears   |
 |  4 |Click `Manage Term` option      | Verify that a Term management dialouge card appears   |
 |  5 |Click the `delete` icon in the action column of the Officer table      | Verify that a confirmation pop-up appears  | 
 |  6 |Confirm the deletion     | Verify that the selected officer is deleted from the table  | 

**Post-conditions:**  

 - The user is removed from the `officer` table from Supabase.
 - The number of `Officers` automatically adjusts.
