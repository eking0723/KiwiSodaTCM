## **PJBU-001:** Budget Allocation - Initial

> **Summary:** Verify initial budget set during project creation.  `<br>`

**Preconditions:** 

* User is logged in as Project Manager

Scenario 1

| \# | Step                                              | Expected Behavior                                                           |
| -- | ------------------------------------------------- | --------------------------------------------------------------------------- |
| 1  | Navigate to the Projects and create a new Project | The create Project form is displayed successfully                           |
| 2  | Enter a valid Project name                        | The project name is accepted without validation errors                      |
| 3  | Input an initial budget amount                    | The budget value is accepted and displayed correctly in the input field     |
| 4  | Complete all required project fields              | All required fields accept valid input and not validation errors are shown  |
| 5  | Click Create Project                              | The project is created successfully and a confirmation message is displayed |

**Post-conditions:**

- The project is created successfully with an initial input budget.
- The budget information is displayed correctly in the projects card and budget management page.
