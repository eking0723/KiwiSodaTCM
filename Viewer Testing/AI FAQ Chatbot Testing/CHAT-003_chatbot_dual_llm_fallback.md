## **CHAT-003:** Chatbot Dual LLM Fallback  

> **Summary:** Verify that the chatbot can switch between AI providers (Groq/Gemini) if one fails.  <br>

**Preconditions:** 
- `GROQ_API_KEY` and `GEMINI_API_KEY` are both configured (initially).

Scenario 1: Fallback from Groq to Gemini (System Simulation)

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Trigger a scenario where the Groq API fails (e.g., temporarily invalidating the key or simulation) | Verify that the `processChatMessage` server action catches the error from Groq. | 
 |  2 | Send a message via the chat window | Verify that the `Thinking...` state remains active while the fallback logic executes. | 
 |  3 | Observe the successful response | Verify that the response is returned from Gemini (provider logged as "Gemini (Fallback)" in server logs). | 
 |  4 | Observe the UI behavior | Verify that the user experience remains seamless without showing a connection error to the user. | 

Scenario 2: Total failure

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Simulate a failure in both Groq and Gemini APIs | Verify that the chatbot returns a graceful error message: "Sorry, I'm having trouble connecting to the server right now. Please try again later." | 

**Post-conditions:**  
 - Chatbot maintains high availability through provider redundancy.
 - Errors are logged on the server side for monitoring.

