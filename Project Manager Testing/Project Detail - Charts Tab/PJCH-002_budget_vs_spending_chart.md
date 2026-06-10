## **PJCH-002:** Budget vs Spending Chart  

> **Summary:** Verify visualization comparing allocated budget vs current expenses.  <br>

**Preconditions:** 
- Project has an allocated budget and some recorded expenses.

Scenario 1: Comparing budget metrics

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Navigate to the `Charts` tab and ensure `Budget vs Spending` is active | Verify that a Bar Chart appears with "Project Budget" on the X-axis. | 
 |  2 | Hover over the `Total Budget` bar | Verify it shows the correct amount (e.g., ₱50,000). | 
 |  3 | Hover over the `Spent Budget` bar | Verify it shows the correct spent amount (e.g., ₱10,000). | 
 |  4 | Observe the Y-axis formatting | Verify that large values are formatted with "k" (e.g., 50k instead of 50,000). | 

**Post-conditions:**  
 - Chart data matches the `total_budget` and `spent_budget` columns in the `projects` table.
 - Visual comparison correctly indicates the utilization percentage.

