## **PROF-003:** Profile Testing - Change Full Name  

> **Summary:** Verify that full name was changed successfully.  <br>

**Preconditions:** User must be logged in.  

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Click `Profile` dropdown at the right side part of the header    | Verify that a dropdown interface appear   |  
 |  2 |Click `View Profile`       | Verify that the user redirects to the Profle Setting page   |  
 |  3 |Enter a new `full name`    | Verify that the the changes instantly reflects in the `Student Name` section   |  
 |  4 |Click `Save Changes` button      | Verify that the profile name has changed successfully   |  
 |  5 |Go back to the main dashboard     | Verify that the profile name in the right side of the header has changed   |  

**Post-conditions:**  

 - User's profile name has been changed in the `profile`
 - User's `full_name` has changed in the Supabase
