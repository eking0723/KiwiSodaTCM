## **TERM-001:** Term Testing - Add Term  

> **Summary:** Verify that user adds new term successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: 12345678)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Term Management` on the navigation bar     | Verify that the user is redirected to the `Term Management` page   | 
 |  3 |Click `Add Term` button   | Verify that a dialouge card appears   |  
 |  4 |Set the `Term Name` to "2026-2027"      | Verify that the text is saved in the input field  |  
 |  5 |Set the `Start Date` to "8/10/2026"      | Verify that the text is saved in the input field   |  
 |  6 |Set the `End Date` to "5/30/2027"      | Verify that the text is saved in the input field  | 
 |  9 |Click `Create Term and Save` button      | Verify that the term appears in the term table            | 
**Post-conditions:**  

 - Term that contains the name, start date, and end date is saved in the Supabase
