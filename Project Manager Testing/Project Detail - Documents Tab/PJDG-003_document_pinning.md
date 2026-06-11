## **PJDG-003:** Document Pinning

> **Summary:** Verify pinning documents for public visibility on the student preview.  `<br>`

**Preconditions:** 

* User is logged as project manager
* A project exists in the system
* At least one document has been uploaded to the project's document

Scenario 1

| \# | Step                                                          | Expected Behavior                                                               |
| -- | ------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| 1  | Navigate to the target project's Documents page               | The Documents page loads successfully and displays available project documents. |
| 2  | Locate a document that is not currently pinned.               | The document is displayed with an option to pin it.                             |
| 3  | Click the**Pin** button/icon for the selected document. | The system processes the request and displays a success message.                |
| 4  | Verify the document's status in the document list.            | The document is marked as**Pinned** or displays a pin indicator.          |

**Post-conditions:**

- The selected document is marked as pinned.
