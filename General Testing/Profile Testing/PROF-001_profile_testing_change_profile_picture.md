## **PROF-001:** Profile Testing - Change Profile Picture  

> **Summary:** Verify that profile picture was added successfully.  <br>

**Preconditions:** 
- User must be logged in. 
- User may or may not have a profile picture

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Click `Profile` dropdown at the right side part of the header    | Verify that a dropdown interface appear   |  
 |  2 |Click `View Profile`       | Verify that the user redirects to the Profle Setting page   | 
 |  3 |Click on the `profile picture`      | Verify that a file upload dialouge appears in the screen  |  
 |  4 |Upload a compatible image file (png or jpeg)     | Verify that the profile thumbnail is changed   |  
 |  5 |Click `Save Changes` button      | Verify that the profile picture has changed successfully  |  
 |  6 |Go back to the main dashboard      | Verify that the small avatar in the right side of the header has changed   |  

**Post-conditions:**  

 - Updates the old profile picture with new profile
 - Updates the avatar url in the Supabase  
 
