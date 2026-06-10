## **CHAT-002:** Chatbot Session Persistence  

> **Summary:** Verify that the chat history is preserved during the current browser session.  <br>

**Preconditions:** 
- User has engaged in a conversation with the chatbot.

Scenario 1: Refreshing the page

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Send a message to the chatbot and receive a response | Verify that the conversation history is displayed. | 
 |  2 | Refresh the browser page (`F5`) | Verify that the chat window (if open) or the chat state is restored from `sessionStorage`. | 
 |  3 | Open the chat window | Verify that the previous messages and responses are still visible in the same order. | 

Scenario 2: Role change / Account switch

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Log out and log in as a different user (or switch to Guest) | Verify that the chat history is cleared (reset to initial message) if the `user_id` stored in `sessionStorage` changes. | 

**Post-conditions:**  
 - Chat history is stored in `sessionStorage` under the key `faq_messages`.
 - History is cleared upon user identity change to ensure privacy.

