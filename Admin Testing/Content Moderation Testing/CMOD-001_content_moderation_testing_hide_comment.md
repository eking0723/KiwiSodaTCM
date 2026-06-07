## **CMOD-001:** Content Moderation Testing - Hide Comment  

> **Summary:** Verify that user was able to hide comment/s successfully.  <br>

**Preconditions:** 
- Device must be connected to the internet
- User must be logged in as `Admin` 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Log in as `Admin` using these credentials: (email: 22-1-02276@vsu.edu.ph ; password: password8086)      | Verify that the user is successfully logged in as Admin | 
 |  2 |Click `Content Moderation` on the navigation bar     | Verify that the user is redirected to the `Content Moderation` page   |
 |  3 |Click on the `Hide` button in the action column      | Verify that the button changes from `Hide` to `Unhide`  | 
 |  4 |Observe the content of the comment in `Comment` column      | Verify that the content has red line signifying that the comment was successfully hiden     | 
 
**Post-conditions:**  

 - The `is_hidden` attributes is updated in the Supabase.
