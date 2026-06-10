## **NOTI-005:** PM: Overdue Task Warnings  

> **Summary:** Verify PM receives daily summaries of missed deadlines when enabled.  <br>

**Preconditions:** 
- User is logged in as Project Manager.
- User is on the `Settings` page.

Scenario 1: Toggling overdue warnings

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Locate the `Overdue Task Warnings` toggle | Verify it is visible for PM role. | 
 |  2 | Toggle the setting and click `Save Changes` | Verify it is saved in `overdue_task_alerts` column. | 
 |  3 | Observe system behavior | Verify that the `deadline-alerts` Edge Function respects this preference. | 

**Post-conditions:**  
 - Daily task status checks are filtered by this preference.

