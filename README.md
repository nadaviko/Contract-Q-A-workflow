AI agent — one that reads contracts and answers questions about them in plain language.

A Contract Q&A Chatbot.

Here's the scenario: a user uploads a contract PDF, types a question, and the agent reads the document and replies with a direct answer — payment terms, termination clauses, renewal conditions, all of it.
No scrolling through 40 pages. No legal background required.

Here's how the pieces connect:

A Chat Trigger — listens for the user's message and receives the uploaded file
Extract From File — pulls readable text out of the PDF so the AI can work with it
An AI Agent — takes the user's question + the extracted text, reasons over both, and writes a response
An OpenAI Chat Model — the actual intelligence powering the reasoning
