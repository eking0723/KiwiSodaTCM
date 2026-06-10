## **PLAT-001:** Platform Setting Testing - Office Information  

> **Summary:** Verify that office informations changed successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: 12345678)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Platform Settings` on the navigation bar     | Verify that the user is redirected to the `Platform Settings` page   |
 |  3 |Enter "OnTrack" in the `Organization Name` input field     | Verify that the text is saved in the field  | 
 |  4 |Enter "USSO" in the `Office Location` input field     | Verify that the text is saved in the field  | 
 |  5 |Enter "ontrack@gmail.com" in the `Contact Email` input field     | Verify that the text is saved in the field  | 
 |  6 |Click `Save Office` button       | Verify that the inputs are saved successfully  |  

**Post-conditions:**  

 - The Organization Name, Office Location, and Contact Email has been updated in the Supabase.  