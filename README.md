# AI Conversational ChatBot on Zoom

For me, Zoom was just for meeting stuff. I never imagined that I would build an AI Chatbot on it. Isn’t it amazing to have a bot that can assist you with your queries during virtual meetings(especially when you're sleeping in between the meetings)? I'm a student. So if you ask me, yes!!! It is a crazy thing. 
That’s what my next project is about!!

I built another AI chatbot, (oh, wait)...

An **Intelligent AI ChatBot** that provides helpful responses to user queries on a wide range of topics within their Zoom conversation discussions by using Cerebras' advanced language models on the Zoom Developers’ platform. 

### Functionalities:

* Responds to user messages in Zoom Team Chat using Cerebras' language models.
* Maintains conversation history for context-aware responses.
* Can be used in direct messages or invoked in group chats and channels.
* Provides helpful information, answers questions, assists with tasks, and engages in discussions on various topics with exceptional speed and accuracy.
* At the end, I will share my experience on how My Bot assisted me during the project when I got stuck.

### Architecture:

![image](https://github.com/user-attachments/assets/e6f02d29-09f2-4af4-b86d-0e423e084716)


Without wasting time on boring talk, let’s start with hands-on.
So, Shall we start?

1.  Let’s Download or update zoom, IF you haven’t:




2. Steps to download Ngrok:
    
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

3. Moving onto the [Zoom Developer Platform:](https://developers.zoom.us/)

Create a Team Chat App:

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

* You can also launch your app in Zoom Team Chat with configured shortcuts that will trigger the defined action. 

  <img width="714" alt="Screenshot 2024-11-16 at 2 12 41 AM" src="https://github.com/user-attachments/assets/003bfbb0-f72f-4b8e-ab09-902675bcac3b">

-It should look like this:
  <img width="312" alt="Screenshot 2024-11-16 at 2 13 21 AM" src="https://github.com/user-attachments/assets/5b96dd0d-e4df-4c44-bd83-45e42b83753a">



4. Setting up a webhook receiver:

   * refer server.js
   * To use this: First install node
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

5. Create a new file .env:
   ```
   ZOOM_CLIENT_ID=your_zoom_client_id
   ZOOM_CLIENT_SECRET=your_zoom_client_secret
   ZOOM_BOT_JID=your_zoom_bot_jid
   CEREBRAS_API_KEY=your_cerebras_api_key
   ```

6. Send ChatBot Message:

   * Refer sendMessage.js
   * Generating an Access token (refer token.js)


7. Let's move onto [Cerebras:](https://inference-docs.cerebras.ai/quickstart)

   * Install the Cerebras Inference library
     ```
     npm install @cerebras/cerebras_cloud_sdk
     ```

   * Create Cerebras file

     refer cerebras.js

8. What next?

Nothing, Your Conversation ChatBot is ready!!! 
Your chatbot will now have a conversation history, which will enable it to end up being more logical and less awkward. As a part of the code, previous messages are saved in memory and attached each time to the subsequent requests to the Cerebras API. This will help the AI to grasp the flow of the conversation and be able to recall what has been said before in the conversation.

You know, what was the best part?
I was stuck in between the coding part, my Bot motivated me by saying kind words. 

<img width="1181" alt="Screenshot 2024-11-16 at 2 24 06 AM" src="https://github.com/user-attachments/assets/387ca009-a338-47ed-b2d2-bbb779058da1">

That was my experience with AI tools. Tell me about your story with AI...












