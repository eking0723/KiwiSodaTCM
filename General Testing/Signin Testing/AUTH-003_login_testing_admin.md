## **AUTH-003:** Login Testing - Admin  

> **Summary:** Verify that user was able to log in as a admin  <br>

**Preconditions:** Account exists in the system with valid email address.

Scenario 1: Entering valid credentials

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Launch the website OnTrack      | Verify that the user redirects to the landing page   | 
 |  2 |Click `Login` Button at the right side of the header      | Verify that the user redirects to the Login page   | 
 |  3 |Enter valid email credential (VSU email)      | Verify that the email input field border is green (valid email entry)   |  
 |  4 |Enter password      | Verify that the password input field border is green (valid password entry)   |
 |  5 |Click the eye icon     | Verify that the password entered is shown  |
 |  6 |Clck `Sign In` button     | Verify that the user redirects to the `admin` dashboard page   |


**Post-conditions:**  
 - User is authenticated in the Supabase authentication  
 - Directed to the `admin` dashboard  
