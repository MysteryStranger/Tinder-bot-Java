# Hello thee and welcome to my little marathon of Java and AI telegram bot
Here we whave a bot with some functions so take a look
it was a marathon by Java Rush 
Here we can take a speak with a bot, try to get a date and also date some famous! 
We work with java development Kit (JDK)
Telegram Bot Project

This bot is a virtual user in Telegram that interacts with people in a human-like way. The bot is designed to:

Engage in conversations
Practice dating interactions
Generate fun and relevant dating profiles
Offer advice for online dating conversations
The bot uses ChatGPT for smart responses and interactions.

Setup Guide

Before coding, prepare your environment:

Install Java Development Kit (JDK)
Use IntelliJ IDEA Community Edition for development
Have Telegram installed (desktop version recommended for testing)
Steps to Start the Project

Download IntelliJ IDEA from the official website and open the project template.
Navigate to TinderBolt -> src -> main -> Java -> com -> telegram to access the necessary Java files.
Run the project in IntelliJ by selecting the class TinderBoltApp and hitting the run button.
Basic Java Example

Java code is structured in a simple way:
public class Main {
   public static void main(String[] args) {
       System.out.println("This is my program");
   }
}

This code prints "This is my program" to the console.

First Features to Implement

The bot responds to /start command by sending a greeting message and an image.
To send messages with buttons, use:
sendTextButtonMessage("Choose mode", "Start", "btn_start", "Stop", "btn_stop");

To send images, use:
sendPhotoMessage("image_name");

Working with Commands

Commands in Telegram (like /start) allow the bot to perform actions. Here’s how to check and respond to a /start command:

if (message.startsWith("/start")) {
    sendPhotoMessage("main");
    sendTextMessage("Welcome to the bot");
    return;
}

Connecting ChatGPT

For smart responses, the bot uses ChatGPT via an API token. To switch the bot to the GPT mode:

if (message.startsWith("/gpt")) {
    currentMode = DialogMode.GPT;
    sendTextMessage("ChatGPT is ready. Ask anything!");
    return;



Profile Creation

The bot can generate Tinder profiles by using the /profile command. User input is processed through ChatGPT to create a personalized profile.
hope you enjoy :)

}![Screenshot 2024-10-07 044524](https://github.com/user-attachments/assets/561d8c24-4f0c-4885-9ef8-68eb77ebfe79)
![Screenshot 2024-10-07 044539](https://github.com/user-attachments/assets/e147f0b4-f1ff-4f8d-933b-3031a12fe9e7)
![Screenshot 2024-10-07 044557](https://github.com/user-attachments/assets/afe71f5b-de90-4e4c-934f-311cd29a8391)
![Screenshot 2024-10-07 044457](https://github.com/user-attachments/assets/240c9480-38cc-4ede-964a-1d28bbb14cab)
