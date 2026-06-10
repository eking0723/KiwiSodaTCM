## **PLAT-005:** Platform Setting Testing - Cookie Policy  

> **Summary:** Verify that cookie policy changed successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: 12345678)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Platform Settings` on the navigation bar     | Verify that the user is redirected to the `Platform Settings` page   |
 |  3 |Copy and Paste this text in to the `Cookie Policy` input field: "Cookie Policy Policy 1: Codition 1"  | Verify that the text is saved in the field    |
   
 |  4 |Click `Save Legal` button      | Verify that the text is saved successfully   |
 |  5 |Navigate to the `Footer` of the page and click on `Cookie Policy`     | Verify that the user is redirected to `Cookie Policy` page  |
 |  6 |Observe the content of the page      | Verify that the updated `Cookie Policy` appears in the page   |

**Post-conditions:**  

 - Upadated the `Cookie Policy` in the Supabase.

