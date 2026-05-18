This is an AI agent 

One that reads contracts and answers questions about them in plain language.

A Contract Q&A Chatbot.

Here's the scenario: a user uploads a contract PDF, types a question, and the agent reads the document and replies with a direct answer — payment terms, termination clauses, renewal conditions, all of it.
No scrolling through 40 pages. No legal background required.

Here's how the pieces connect:

A Chat Trigger — listens for the user's message and receives the uploaded file

Extract From File — pulls readable text out of the PDF so the AI can work with it

An AI Agent — takes the user's question + the extracted text, reasons over both, and writes a response

An OpenAI Chat Model — the actual intelligence powering the reasoning

Prerequisites

Make sure you have all four of these before starting:

✅ An n8n account — sign up free at n8n.io, the cloud version works fine. 

✅ An OpenAI API key — go to platform.openai.com, create an account, and generate a key under API Keys. 

✅ The starter workflow file — download the file Contract Q&A workflow.json

✅ The sample contract PDF — download the sample contract (a fictional vendor agreement for this lab)
                [Aurelios System NDA 1.pdf](https://github.com/user-attachments/files/27938544/Aurelios.System.NDA.1.pdf)

Ways to build this

    Step 1. Create a new workflow.

       Open your n8n account and click "Create Workflow" in the top right. You'll land on a blank canvas — this is your build surface.
 
   Step 2. Import the starter file.

      Click the three-dot menu (⋮) at the top right, select "Import from File", and upload the n8n-workflow.json file from the prerequisites.

      Your canvas will populate with all the nodes already connected.

  Step 3. Verify the connections.

      Every node should be linked with a visible line. If anything looks disconnected, drag the small circle on the right edge of that node and connect it to the next one.

 Step 4. Add your OpenAI API key.

      Click the "OpenAI Chat Model" node. In the settings panel, click "Credential" → "Create New Credential" → paste your API key → Save.

      n8n encrypts and stores it. You won't need to paste it again across any of the labs.

  Step 5. Open the chat and test.

     Click "Open Chat" at the bottom of the canvas. Upload the sample contract PDF and ask: "What are the payment terms?"

     Jump to the Testing Your Agent section at the bottom to try more questions.

Process Flow

<img width="1283" height="239" alt="Screenshot 2026-05-17 at 5 03 57 PM" src="https://github.com/user-attachments/assets/47baa077-d179-4a40-a21a-213a1feb978e" />
