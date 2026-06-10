## **PJCH-001:** Team Performance Chart  

> **Summary:** Verify Recharts bar chart for member task completion.  <br>

**Preconditions:** 
- Project has members with assigned tasks (some completed, some pending).

Scenario 1: Viewing team performance

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Navigate to the `Charts` tab and ensure `Team Performance` is active | Verify that a Bar Chart appears with member names on the X-axis. | 
 |  2 | Hover over a bar in the chart | Verify that a tooltip appears showing the exact number of `Assigned` and `Completed` tasks for that member. | 
 |  3 | Observe the bar colors | Verify that `Assigned` tasks are colored yellow and `Completed` tasks are colored green. | 

**Post-conditions:**  
 - Chart data matches the task counts in the `tasks` table.
 - Legend correctly identifies the data series.
