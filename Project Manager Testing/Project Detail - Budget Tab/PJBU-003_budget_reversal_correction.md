## **PJBU-003:** Budget Reversal/Correction

> **Summary:** Verify reversing or correcting approved expenses/allocations.  `<br>`

**Preconditions:** 

* User is logged in as project manager
* A project exists with an allocated budget
* At least one approved expense or budget allocation exists in the project.

Scenario 1

| \# | Step                                                                | Expected Behavior                                                       |
| -- | ------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| 1  | Navigate to the specific project's budget tracking                  | The budget tracking page loads and displays project budget information  |
| 2  | Locate an approved expense record                                   | The approved expense is visible in the expense list                     |
| 3  | Select the specific expense and click the "Reverse / Correct Entry" | A confirmation dialog is displayed                                      |
| 4  | Confirm the reversal action                                         | The system processes the request                                        |
| 5  | Review the project's budget summary                                 | The reversed expense amount is removed from the total expenses          |
| 6  | Verify the remaining budget                                         | The remaining budget is increased by the amount of the reversed expense |

**Post-conditions:**

- The selected expense is successfully reversed
- Budget totals are recaulculated accurately.
