## **PLAT-004:** Platform Setting Testing - Terms and Conditions  

> **Summary:** Verify that terms and conditionschanged successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: password8086)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Platform Settings` on the navigation bar     | Verify that the user is redirected to the `Platform Settings` page   |
 |  3 |Copy and Paste this text in to the `Terms and Conditions` input field: "Terms and Conditons Term 1: Codition 1"  | Verify that the text is saved in the field    |
   
 |  4 |Click `Save Legal` button      | Verify that the text is saved successfully   |
 |  5 |Navigate to the `Footer` of the page and click on `Terms and Conditions`     | Verify that the user is redirected to `Terms and Conditions` page  |
 |  6 |Observe the content of the page      | Verify that the updated `Terms and Conditions` appears in the page   |

**Post-conditions:**  

 - Upadated the `Terms and Conditions` in the Supabase.
