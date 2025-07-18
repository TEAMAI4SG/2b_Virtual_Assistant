# 02b. 🤖 Create Your Own Virtual Assistant
## 💻 BUS 118I Digital Innovation

---

## 🎯 Learning Goal: 
- Important skills to Watson Assistant instance
- Launch your Watson Assistant

---

## ⏱️ Estimated time: 
- 30 minutes

---

## 🪜 Steps: 

## 🧩 Milestone 1: Create or Finding existing Watson Assistant Service

1. Login to IBM Cloud. [https://cloud.ibm.com]
2. Find the Watson Assistant you created in Lab 1. Click on the **Magnifier** left to **Catalog** 

![Picture 1](screenshots/pic1.png) 

Search for **“Watson Assistant”** and I see **“Watson Assistant-cq”** pop up and I click on that. You probably have a different name from mine. The code after “Watson Assistant” is randomly generated but you can always change it. You may have multiple Watson Assistant services. Or if you don’t have any, please go ahead and create a Watson Assistant as you did in the previous lab.

![Picture 2](screenshots/pic2.png) 

3. After clicking on **“Watson Assistant-cq”** (or a different name that you might have), you will see the home page for this Watson Assistant. Click on “Launch Watson Assistant”. A new window will open and it takes a few seconds to load the Watson Assistant.

![Picture 3](screenshots/pic3.png)

---

## 🆕 Milestone 2: Create an assistant

4. Click **“Create new +”** in the drop down arrow next to COVID Crisis Communication. 

![Picture 4](screenshots/pic4.png) 

5. Name the Watson Assistant instance “My Second Assistant”, and click on **“Create assistant”.**

![Picture 5](screenshots/pic5.png)

6. On the side bar, click on **“Assistant settings”.**

![Picture 6](screenshots/pic6.png) 

7. Scroll down and click on **“Activate dialog”**. Click on “**Activate dialog”** again on the pop-up.

![Picture 7](screenshots/pic7.png)


8. On the side bar, click on the new **Dialog** button.

![Picture 8](screenshots/pic8.png)

---

## ⚙️ Milestone 3: Start a dialog skill

9. You are now in the page for the skill

![Picture 9](screenshots/pic9.png) 

---

## 📚 Milestone 4: Add Intents from Content Catalog

10. Click the **Content Catalog** tab, the last tab on the left navigation bar. Find **General** in the list, and then click **Add content**.

![Picture 10](screenshots/pic10.png)


11. Open the **Intents** tab to review the intents and associated example utterances that were added to your training data. You can recognize them because each intent name begins with the prefix #General_. You will add the #General_Greetings and #General_Ending intents to your dialog in the next step.

![Picture 11](screenshots/pic11.png)

---

## 🏗️ Milestone 5: Build a dialog

12. In the Watson Assistant tool, click the **Dialog** tab and “**Create dialog +”.**

![Picture 12](screenshots/pic12.png)


You see two nodes:
- **Welcome:** Contains a greeting that is displayed to your users when they first engage with the assistant.
- **Anything else:** Contains phrases that are used to reply to users when their input is not recognized.

![Picture 13](screenshots/pic13.png)

13. Click the **Welcome node** to open it in the edit view. Replace the default response with text, “Welcome to the Watson Assistant tutorial! I am a chat bot created by your name”. And close the edit view.

![Picture 14](screenshots/pic14.png)

14. Click the **Try it** icon to open the “Try it out” panel. You should see your welcome message. Note: If your message is not showing up, select “Clear”. 

![Picture 15](screenshots/pic15.png)

15. Click on the **three dots** on the Welcome node, and then select **Add node below**. Type #General_Greetings in the “Enter condition” field of this node. Then, select the #General_Greetings option. Add the response, “Good day to you!” Close the edit view.

![Picture 16](screenshots/pic16.png)

![Picture 17](screenshots/pic17.png)

16. Click on the **three dots** on the new “#General_Greetings” node, and then select **Add node below** to create a peer node. In the peer node, specify **#General_Ending** as the condition, and “OK. See you later.” as the response. Close the edit view.

 ![Picture 18](screenshots/pic18.png) 

17. You built a simple dialog to recognize and respond to both greeting and ending inputs. Let's see how well it works. Click the **Try it** icon to open the **"Try it out"** pane. There's that reassuring welcome message. At the bottom of the pane, type **Hello** and press **Enter**. The output indicates that the #hello intent was recognized, and the appropriate response (Good day to you.) appears. Try the following input:
- bye
- howdy
- see ya
- good morning
- Sayonara

Watson can recognize your intents even when your input doesn't exactly match the examples that you included. The dialog uses intents to identify the purpose of the user's input regardless of the precise wording used, and then responds in the way you specify.


18. On the side bar, click on **Upload / Download** and under the **Download** tab click the blue **Download button**. 


![Picture 19](screenshots/pic19.png)


19. An assistant is a cognitive bot to which you add a skill that enables it to interact with your customers in useful ways.

![Picture 20](screenshots/pic20.png)

- Click on the drop down arrow next to **My Second Assistant** tab.
- Click **“Create New +”.**
- Name the assistant, **Assistant Tutorial.**
- Click **Create assistant**.

---

## 💾 Milestone 6: Add Dialog Skill to Assistant
 
20. From the new assistant page, click **Dialog** on the side bar. Navigate to **Upload / Download** and under the **Upload** tab upload the My-Second-Assistant-dialog.json file you just downloaded from the My Second Asisstant chatbot and click on **“Upload and replace”** on the pop-up. 


![Picture 21](screenshots/pic21.png)

---


## 🚀 Milestone 7: Launch the Watson Assistant

21. Click on **Preview** on the side bar. 

![Picture 22](screenshots/pic22.png)

22. On the “Preview assistant” page, click on **“Customize web chat”.**

![Picture 23](screenshots/pic23.png)

23. Select the “Home screen” tab and switch the setting from on to off. 

![Picture 24](screenshots/pic24.png)

24. Back on the “Preview assistant” page, you can see how your chatbot will look to users on the right hand side. Copy and open the URL generated under **“Copy link to share”.** The page opens in a new tab. Say hello to your assistant, and watch it respond. You can share the URL with others who might want to try out your assistant.

![Picture 25](screenshots/pic25.png)

![Picture 26](screenshots/pic26.png)



---

## 📸 Deliverables:

**Please read the following instructions carefully to receive full credit. After taking two screenshots, one from Milestone 3 and one from Milestone 7, please add the screenshots in a Word document and turn it in on Canvas for Lab 2.**

**Tip:** If your login box ever covers the content, then please zoom out within your browser window with Ctrl + - or Cmd + -

## Milestone 3: Create a dialog skill

1. **After completing milestone 3**, please take a screenshot of your Watson Assistant and its dialog. **(Important: Please click on the person icon on the upper right corner to show your name in the screenshot otherwise you will not receive credit.)**

![Picture 27](screenshots/pic27.png) 

## Milestone 7: Integrate the Assistant

1. After completing Milestone 7, please have a conversation with your chatbot  **within the Preview link** (another webpage or opened on your smartphone’s browser) by greeting your chatbot with “Hello” and saying goodbye to your chatbot, such as “Talk to you next time” or “Goodbye.” Please take a screenshot of your whole conversation. **(Important: Please ensure that your name is placed within the chat conversation noted in the Discrepancies and Modifications step 3a above to receive full credit.)**

![Picture 28](screenshots/pic28.png)

---

## 🎉 Congratulations! - You've successfully created, trained, and launched your own Watson Assistant chatbot. Great job bringing your virtual assistant to life! 🌟



