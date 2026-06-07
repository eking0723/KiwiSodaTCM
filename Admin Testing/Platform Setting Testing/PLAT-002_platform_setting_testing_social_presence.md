## **PLAT-002:** Platform Setting Testing - Social Presence  

> **Summary:** Verify that social presence informations changed successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: password8086)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Platform Settings` on the navigation bar     | Verify that the user is redirected to the `Platform Settings` page   |
 |  3 |Enter "ontrack.facebook.com" in the `Facebook` input field     | Verify that the text is saved in the field  | 
 |  3 |Enter "@ontrackinsta" in the `Instagram` input field     | Verify that the text is saved in the field  |  
 |  3 |Click `Save Socials` button       | Verify that the inputs are saved successfully  |  

**Post-conditions:**  

 - The Facebook and Instagram socials has been updated in the Supabase.  
