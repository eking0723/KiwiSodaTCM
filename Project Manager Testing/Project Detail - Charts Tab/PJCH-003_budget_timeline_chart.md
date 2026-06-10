## **PJCH-003:** Budget Timeline Chart  

> **Summary:** Verify visualization of project balance trends over time.  <br>

**Preconditions:** 
- Project has multiple entries in the `budget_logs` table (budget history).

Scenario 1: Viewing balance trends

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Navigate to the `Charts` tab and ensure `Budget Timeline` is active | Verify that an Area Chart appears with dates on the X-axis. | 
 |  2 | Observe the chart line | Verify it shows the project's total balance (or remaining) at each log entry point. | 
 |  3 | Hover over a point on the line | Verify a tooltip shows the date and the balance at that time. | 
 |  4 | Observe the gradient fill | Verify that the area under the line has a professional green gradient. | 

**Post-conditions:**  
 - Chart data correctly reflects the chronological history of the budget.
 - Area chart accurately visualizes the "burn rate" or balance growth.

