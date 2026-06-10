## **PJTT-004:** Task Cost Budget Impact  

> **Summary:** Verify that assigning a cost to a task updates the project's spent budget and logs.  <br>

**Preconditions:** 
- User is logged in as Project Lead.
- Project has sufficient remaining budget.

Scenario 1: Assigning a task with a cost

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Open the `Assign Task` dialog | Verify that the `Budget Cost (Optional)` field is visible. | 
 |  2 | Enter a cost (e.g., ₱2,000.00) and select an `Expense Category` | Verify that the cost is within the remaining balance. | 
 |  3 | Complete the task assignment and click `Create Task` | Verify that the task is created successfully. | 
 |  4 | Navigate to the `Budget` tab | Verify that the `Budget Used` has increased by ₱2,000.00. | 
 |  5 | Observe the `Budget Audit Trail` | Verify that a new entry appears with reason: "Task Allocation: Assigned Task - [Title]". | 

**Post-conditions:**  
 - Spent budget is automatically updated in the `projects` table.
 - A corresponding entry is added to the `budget_logs` table.

