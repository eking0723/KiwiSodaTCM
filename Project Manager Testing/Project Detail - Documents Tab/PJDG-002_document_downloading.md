## **PJDG-002:** Document Downloading

> **Summary:** Verify that uploaded documents can be downloaded by authorized users.  `<br>`

**Preconditions:** 

* User is logged as project manager
* A project exists in the system
* At least one document has been uploaded to the project's document

Scenario 1

| \# | Step                                                | Expected Behavior                                                                                                                               |
| -- | --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| 1  | Navigate to the target project's Documents page.    | Verify that ...                                                                                                                                 |
| 2  | Locate an uploaded document in the document list.   | Verify that ...                                                                                                                                 |
| 3  | Click the "Cloud download" button or document link. | Verify that ...                                                                                                                                 |
| 4  | Verify the downloaded file name and format.         | The file opens correctly, its contents match the uploaded document, and the file name and file extension match the original uploaded document. |

**Post-conditions:**

- The selected document is successfully downloaded.
- The downloaded file matches the original uploaded document.
- z
