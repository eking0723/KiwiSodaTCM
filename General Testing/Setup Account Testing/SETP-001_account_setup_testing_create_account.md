## **SETP-001:** Account Setup Testing - Create Account  

> **Summary:** Verify that user was able to setup an account successfully.  <br>

**Preconditions:** 
- User must have VSU gmail account.
- Device must be connected to internet. 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Launch the website OnTrack      | Verify that the user redirects to the landing page   | 
 |  2 |Click `Login` Button at the right side of the header      | Verify that the user redirects to the Login page   | 
 |  3 |Click `Continue with Google` button      | Verify that user redirects to Google Authentication  |  
 |  4 |Enter valid VSU gmail credentials (email and password) and click `Done`  | Verify that the user redirects to the Setup page  | 
 |  5 |Enter `Full name` credential      | Verify that full name is saved in the full name input field  | 
 |  6 |Enter `Username` credential     | Verify that username is saved in the username input field    | 
 |  7 |Enter valid new password (at least 8 characters)      | Verify that new password is saved in the new password input field   | 
 |  8 |Click `Complete Setup` button      | Verify that user redirects to the Dashboard page   | 
**Post-conditions:**  

 - User account is created in Supabase  
 - Default profile information is created with `viewer` type in Supabase   
