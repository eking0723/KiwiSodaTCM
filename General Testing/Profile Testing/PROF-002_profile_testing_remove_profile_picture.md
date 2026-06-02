## **PROF-002:** Profile Testing - Remove Profile Picture  

> **Summary:** Verify that profile picture was changed successfully.  <br>

**Preconditions:** 
- User must be logged in. 
- User must have an existing profile picture

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Click `Profile` dropdown at the right side part of the header    | Verify that a dropdown interface appear   |  
 |  2 |Click `View Profile`       | Verify that the user redirects to the Profle Setting page   | 
 |  3 |Click `Remove Picture` button     | Verify that the profile thumbnail has been removed  |   
 |  4 |Click `Save Changes` button      | Verify that the profile picture has been removed successfully  |  
 |  5 |Go back to the main dashboard      | Verify that the small avatar in the right side of the header has changed in to default avatar  |  

**Post-conditions:**  

 - Removes the current profile picture
 - Updates the avatar url in to `null` in the Supabase  
 
