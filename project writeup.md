
### 1.  Let’s Download or update Zoom, If you haven’t:

<img width="1470" alt="Screenshot 2024-11-16 at 2 34 14 AM" src="https://github.com/user-attachments/assets/f6832d9b-68e4-4386-87e7-47c1a3b3e51d">


### 2. Steps to download Ngrok:
    
   * Installation: For [MacOS](https://ngrok.com/docs/getting-started/?os=macos)
   * Sign up for an [ngrok](https://dashboard.ngrok.com/get-started/setup/macos) account.
   * Copy your [ngrok authtoken](https://dashboard.ngrok.com/get-started/your-authtoken) from your ngrok dashboard.

Run the following command in your terminal:      
```
ngrok config add-authtoken <TOKEN>
```
Expose your tunnel:   

```
ngrok http http://localhost:4000
```

### 3. Moving onto the [Zoom Developer Platform:](https://developers.zoom.us/)

### **Create a Team Chat App:**

* Create an account on the zoom, Login to Zoom Marketplace. And Assign a name to the Bot.

 <img width="1446" alt="Screenshot 2024-11-16 at 2 07 23 AM" src="https://github.com/user-attachments/assets/d024c815-a688-4513-a6fd-ebc17f71cc51">

* Click on Build App.

   <img width="565" alt="Screenshot 2024-11-16 at 2 04 16 AM" src="https://github.com/user-attachments/assets/1bf0ec89-2567-45a7-a52d-ce3a342f18d9">

* In the surface section, Select where to use that app.

   <img width="792" alt="Screenshot 2024-11-16 at 2 06 25 AM" src="https://github.com/user-attachments/assets/efbcb426-0215-4a7a-a6be-d64caf5ad4fb">

* Enable Team Chat Subscription.

   <img width="729" alt="Screenshot 2024-11-16 at 2 08 55 AM" src="https://github.com/user-attachments/assets/01f43764-d5ce-44cd-8817-5c9ddaaea0a5">

* On the Local Test page, add and preview your app and share it with internal users.

   <img width="781" alt="Screenshot 2024-11-16 at 2 10 30 AM" src="https://github.com/user-attachments/assets/cb712d28-b027-483b-97e5-674971193b4b">


### 4. Setting up a webhook receiver:

   * refer //server.js file.
   * To use this: First install node.
     
  If you do not have node installed, install it first:

   ```
   brew install node@22
   ```

  
  Install Expree:
  ```
  npm install express
  ```


  Run the server:
  ```
  node server.js
  ```


### 5. Create a new file .env:

   ```
   ZOOM_CLIENT_ID=your_zoom_client_id
   ZOOM_CLIENT_SECRET=your_zoom_client_secret
   ZOOM_BOT_JID=your_zoom_bot_jid
   CEREBRAS_API_KEY=your_cerebras_api_key
   ```

### 6. Send ChatBot Message:

   * Refer //sendMessage.js file.
   * Generating an Access token (refer token.js)


### 7. Let's move on [Cerebras:](https://inference-docs.cerebras.ai/quickstart)

    
   * Before diving into Cerebras Inference, you can go through the documentation of AI Agent Bootcamp on the Cerebras site. It helped me to 
     understand the overview of the overall project.You can also explore the components that make up agentic workflows and highlight some 
     key differences in control flow between traditional software and agentic workflows. 
     This makes it a crucial topic for developers interested in building with LLMs.

     <img width="1462" alt="Screenshot 2024-12-08 at 5 00 27 PM" src="https://github.com/user-attachments/assets/131652f3-9552-491d-a593-bb2bf31fb0d4">

   * You will get a brief idea of how to use the Cerebras API in code.

     <img width="1463" alt="Screenshot 2024-12-08 at 5 04 52 PM" src="https://github.com/user-attachments/assets/4fc45a07-f69e-475d-b333-26582c4591d9">


   * Install the Cerebras Inference library

   * Install the Cerebras Inference library
     ```
     npm install @cerebras/cerebras_cloud_sdk
     ```

   * Create Cerebras file

     refer //cerebras.js file.

### 8. What next?

Nothing, Your Conversational ChatBot is ready!!! 

This chatbot will now have a conversation history, which will enable it to end up being more logical and less awkward. As a part of the code, previous messages are saved in memory and attached each time to the subsequent requests to the Cerebras API. This will help the AI to grasp the flow of the conversation and be able to recall what has been said before in the conversation.


* You can also launch your app in Zoom Team Chat with configured shortcuts that will trigger the defined action.
  

  <img width="714" alt="Screenshot 2024-11-16 at 2 12 41 AM" src="https://github.com/user-attachments/assets/003bfbb0-f72f-4b8e-ab09-902675bcac3b">


-It should look like:


  <img width="312" alt="Screenshot 2024-11-16 at 2 13 21 AM" src="https://github.com/user-attachments/assets/5b96dd0d-e4df-4c44-bd83-45e42b83753a">



You know, what was the best part?
I was stuck in between the coding part, my Bot motivated me by saying kind words. 


<img width="1181" alt="Screenshot 2024-11-16 at 2 24 06 AM" src="https://github.com/user-attachments/assets/387ca009-a338-47ed-b2d2-bbb779058da1">



That was my experience with AI tools. I would love to know your story with AI...
