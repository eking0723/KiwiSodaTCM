## **PJDG-004:** Document Deletion

> **Summary:** Verify permanent removal of files from the project and storage.  `<br>`

**Preconditions:** 

* User is logged as project manager
* A project exists in the system
* At least one document has been uploaded to the project's document

Scenario 1

| \# | Step                                             | Expected Behavior                                                               |
| -- | ------------------------------------------------ | ------------------------------------------------------------------------------- |
| 1  | Navigate to the target project's Documents page. | The Documents page loads successfully and displays available project documents. |
| 2  | Locate the document to be deleted.               | The document is visible in the document list.                                   |
| 3  | Click the Trash icon for the selected document.  | A confirmation dialog is displayed.                                             |
| 4  | Review the deletion warning message.             | The system informs the user that the action is permanent and cannot be undone.  |
| 5  | Click "Ok"                                       | The system processes the deletion request and displays a success message.       |
| 6  | Return to the document list.                     | The deleted document no longer appears in the project repository.               |

**Post-conditions:**

- The selected document is permanently removed from the project repository.
- The document can no longer be viewed, downloaded, or accessed through any project page.
