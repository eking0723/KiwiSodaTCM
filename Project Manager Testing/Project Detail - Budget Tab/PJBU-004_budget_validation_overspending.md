## **PJBU-004:** Budget Validation - Overspending

> **Summary:** Verify system prevents recording expenses exceeding the total budget.  `<br>`

**Preconditions:** 

* User is logged as project manager
* A project exists with an allocated budget
* The project has a remaining budget lower than the expense amount to be recorded.

Scenario 1

| \# | Step                                                      | Expected Behavior                                                                         |
| -- | --------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| 1  | Navigate to the target project's Budget Tracking page.    | The Budget Tracking page loads successfully and displays the current budget information.  |
| 2  | Click the "Record Expense" button.                       | Verify that ...                                                                           |
| 3  | Enter an expense amount greater than the remaining budget | Verify that ...                                                                           |
| 4  | Fill all the required fields                              | The category is selected successfully and the description is accepted                     |
| 5  | Click the "Record Expense"button.                         | The system validates the expense against the remaining budget.                            |
| 6  | Return to the expense list and budget summary.            | No new expense record is created and budget values remain unchanged and throws a warning. |

**Post-conditions:**

- The overspending expense record is not saved in the system.
- The project's total expenses remain unchanged.
- An appropriate validation or error message is displayed to the user.
