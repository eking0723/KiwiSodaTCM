## **FPAS-001:** Forgot Password Testing  

> **Summary:** Verify that user was able to change password.  <br>

**Preconditions:** Account exists in the system with valid email address.

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Go to the Login page      | Verify that user redirected to the `Login`  | 
 |  2 |Click `Forgot Password` hyperlink      | Verify that the user is redirected to the `forgot-password` page  | 
 |  3 |Enter valid email credential (VSU email)      | Verify that the email input field border is green (valid email entry)  |
 |  4 |Click `Send Reset Link` button     |Verify that an email containing the reset password confirmation is received from gmail inbox  |
 |  5 |Click `Reset Password` button from the mail      |Verify that the user is redirected to `upadte-password` page       |  
 |  6 |Enter a `new password`       |Verify that the new password is saved in the input field     |  
 |  7 |Click `Update Password` button      |Verify that a successful update message appears and redirects the user to dashboard      |    

**Post-conditions:**  

 - Updates the old password with new password  
