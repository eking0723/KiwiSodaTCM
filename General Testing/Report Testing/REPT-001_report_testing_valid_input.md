## **REPT-001:** Report Testing - Valid Input  

> **Summary:** Verify that reports were successfully uploaded.  <br>

**Preconditions:**
- User must be logged in. 
- Device is connected to the internet.

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 |Navigate to `Support` on the side bar      | Verify that the user is redirected to `Help and Support` page  | 
 |  2 |Click on the `Issue Type` dropdown      | Verify that a dropdown interface appears  | 
 |  3 |Choose a category from the dropdown      | Verify that the category choosen is displayed in the field   | 
 |  4 |Click on the `Priority` dropdown      | Verify that a dropdown interface appears   | 
 |  5 |Choose a priority level      | Verify that the priority level choosen is displayed in the field  | 
 |  6 |Type "System bug" in the `Subject` input field     | Verify that the text is saved the input field   | 
 |  7 |Type "System bug was found!" in the `Description`      | Verify that the entry is saved in the input field   | 
 |  8 |Upload a file in the attachment field      | Verify that file is saved in the attachment field   | 
 |  9 |Click `Send Report` button      | Verify that a message `Report Submitted` appears in the screen   |  

**Post-conditions:**  

 - Report is submitted to the database  
 - Report appeared in project manager and admin personel   
