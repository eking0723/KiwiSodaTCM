## **REPT-002:** Report Testing - Invalid Input  

> **Summary:** Verify that reports were unsuccessfully uploaded.  <br>

**Preconditions:** 
- User must be logged in. 
- Device is connected to the internet. 

Scenario 1 

 | \# | Step | Expected Behavior | 
 |----|------|-------------------|
 |  1 |Navigate to `Support` on the side bar      | Verify that the user is redirected to `Help and Support` page  | 
 |  2 |Leave the `Issue Type` untouched     | Verify that the category input field doesn't have an entry   | 
 |  3 |Click `Send Report` button      | Verify that a message "Please select an item in the list" appears below the `Issue Type` input field  | 
 |  4 |Click on the `Issue Type` dropdown      | Verify that a dropdown interface appears  |  
 |  5 |Choose a category from the dropdown      | Verify that the category choosen is displayed in the field   |  
 |  6 |Click `Send Report` button      | Verify that a message "Please fill out this field" appears below the `Subject` input field  |
 |  7 |Type "System bug" in the `Subject` input field     | Verify that the text is saved the input field   | 
 |  8 |Click `Send Report` button      | Verify that a message "Please fill out this field" appears below the `Description` input field  | 

**Post-conditions:**  

 - Report failed to submit 
