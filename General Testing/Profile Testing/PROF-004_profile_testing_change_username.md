## **PROF-004:** Profile Testing - Change Username  

> **Summary:** Verify that username was changed successfully.  <br>

**Preconditions:** User must be logged in. 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Click `Profile` dropdown at the right side part of the header    | Verify that a dropdown interface appear   |  
 |  2 |Click `View Profile`       | Verify that the user redirects to the Profle Setting page   |  
 |  3 |Enter a new `username`    | Verify that the the changes was saved in the input field  |  
 |  4 |Click `Save Changes` button      | Verify that the username has changed successfully   |   

**Post-conditions:**  

 - User's username has been changed in the `profile`
 - User's `username` has changed in the Supabase 
