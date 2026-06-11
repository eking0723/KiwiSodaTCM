## **PJBU-002:** Expense Recording

> **Summary:** Verify adding manual expense logs with categories and descriptions.  `<br>`

**Preconditions:** 

* User is logged in as project manager
* A project exists with an allocated budget
* The project budget tracking is accessible
* Expense category have been configured in the system (e.g.. Materials, Equipment, Miscellaneous)

Scenario 1

| \# | Step                                                     | Expected Behavior                                                                                                        |
| -- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| 1  | Navigate to the specific project's budget tracking page | The budget tracking page loads succesfully and displayes the current budget information                                  |
| 2  | Click the "Record Expense"                               | The Add Expense form/modal is displayed                                                                                  |
| 3  | Enter a valid expense amount                             | The amount is accepted without validation errors                                                                        |
| 4  | Select an expense category                               | The selected category uis dispayed correctly in the form                                                                 |
| 5  | Enter a description (optional)                           | The description is displayed correctly                                                                                   |
| 6  | Click the "Record Expense" button                      | The expense record is successfully saved                                                                                 |
| 7  | View the project's expense list                          | Verify that the newly added expense appears in the expense list with the correct amount, category, description, and date |
| 8  | Check the project's budget summary                       | Verify that the budget is reduced accordingly                                                                            |

**Post-conditions:**

- The expense record is successfully stored in the system
- The expense appears in the project's expense log
- The total project expenses are updated to include the new expense
- The remaining budget is recalculated and displayed correctly
