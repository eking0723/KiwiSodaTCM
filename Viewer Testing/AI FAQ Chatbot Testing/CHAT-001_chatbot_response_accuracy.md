## **CHAT-001:** Chatbot Response Accuracy  

> **Summary:** Verify that the chatbot provides relevant answers about OnTrack features and live projects.  <br>

**Preconditions:** 
- `GROQ_API_KEY` or `GEMINI_API_KEY` is configured in the environment.
- Live projects exist in the current active term.

Scenario 1: Asking about platform features

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Click the floating `MessageCircle` button (bottom right) | Verify that the chat window opens with an initial greeting from "OnTrack Assistant". | 
 |  2 | Click one of the quick questions (e.g., "How do I track project budget?") | Verify that the question appears as a user message and a "Thinking..." indicator appears. | 
 |  3 | Observe the assistant response | Verify that the response explains the budget tracking feature using professional and helpful tone. | 

Scenario 2: Asking about live projects

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Type "What are the ongoing projects?" in the chat input | Verify that the assistant lists the titles and descriptions of projects currently marked as `Live` in the system. | 
 |  2 | Ask an unrelated question (e.g., "Who won the World Cup?") | Verify that the assistant responds with: "I can only assist with questions related to the OnTrack platform and its projects." | 

**Post-conditions:**  
 - Interactions are logged in the `faq_bot_logs` table for authenticated users.
 - Responses are formatted using Markdown.

