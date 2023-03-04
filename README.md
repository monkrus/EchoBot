# EchoBot

## This bot is a simple echo bot, which means that it listens for incoming messages and then echoes them back to the user who sent the message. When you send a message to the bot, it will reply with the same message.

## The bot is using the Telegram Bot API to communicate with the Telegram servers. It uses the tgbotapi package in Golang to create a bot instance and listen for incoming updates from the Telegram servers. When an update is received, the bot checks if it is a message update and then sends back a reply with the same message to the user who sent the message.

## This bot can be used as a starting point for more complex Telegram bots. You can modify the code to add more functionality, such as sending images, videos, or audio messages, or processing commands from users.

## Install:
## go get github.com/go-telegram-bot-api/telegram-bot-api

## Create a Telegram Bot
## Open Telegram and search for the Botfather.
## Send the command /newbot to create a new bot.
## Follow the instructions to set a name and username for your bot.
## Botfather will give you a token. Copy this token, you will need it later.

## Code the Telegram Bot
## Create a new  main.go 
## Replace <YOUR_BOT_TOKEN> with the token provided by Botfather.

## Run the Telegram Bot
## Open a chat with your bot in Telegram and send it a message.
## You should see the message echoed back to you.

## Deploy on ngrok
## Download and install ngrok.
## Open a new terminal window and navigate to the directory where you saved the ngrok executable.
## Run :
## ngrok http 8080

## Copy the https URL generated by ngrok. It should look like https://<random_string>.ngrok.io.
## Replace the webhook URL in your code with the ngrok URL:

## Copy code
## bot.SetWebhook(tgbotapi.NewWebhook("<ngrok_url>/<your_token>"))

## Test the bot by sending a message to it.
