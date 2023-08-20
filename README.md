# Bard AI Telegram Bot

This repository contains a Telegram bot that utilizes the Generative AI API to respond to user messages with creative and contextually relevant content. The bot employs the `telebot` library for Telegram communication and the `google.generativeai (palm)`library (Bard Ai from Google)  for AI-powered responses.

## Getting Started

To deploy and use the Bard AI Telegram Bot, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/ghaiith/bard-ai-telegram-bot.git
   cd bard-ai-telegram-bot
   ```

2. Install the required dependencies. You can use a virtual environment to keep your dependencies isolated:

   ```bash
   pip install -r requirements.txt
   ```

3. Obtain the necessary API keys:

    - If you don't have a Telegram bot, you can create one by talking to the [BotFather](https://t.me/botfather) on Telegram. Follow these steps:
     - Open Telegram and search for "BotFather."
     - Start a chat with BotFather and use the `/newbot` command.
     - BotFather will ask for a name for your bot. Choose a name for your SheinBot (e.g., "MyChatbot").
     - BotFather will then ask for a username for your bot. The username must end with "bot" (e.g., "MyChatai_bot").
     - Once your bot is created, BotFather will provide you with a bot token. Save this token; you will need it later.

   - Generative AI API Key: You need an API key from the Generative AI service. Sign up and acquire an API key by following the instructions on the [Generative AI Website](https://makersuite.google.com/).

4. Configure the Bot:

   Open the `main.py` file and replace the placeholders with your actual Telegram bot token and Generative AI API key:

   ```python
   TOKEN = 'YOUR_TELEGRAM_BOT_TOKEN'
   palm.configure(api_key="YOUR_GENERATIVE_AI_API_KEY")
   ```

5. Run the Bot:

   Start the bot by running the following command:

   ```bash
   python main.py
   ```

6. Interact with the Bot:

   Send messages to your Telegram bot, and it will respond with creative content generated by the Generative AI model.

## Features

- Responds to `/start`, `/help`, and `/hello` commands with a welcome message.
- Handles user messages by generating contextually relevant responses using the Generative AI model.
- Provides feedback to users when they send an empty message.
- Incorporates default parameters for the Generative AI model, which can be adjusted based on your preferences.

## Contribution

Contributions to this project are welcome! If you find any bugs or have suggestions for improvements, feel free to create issues or submit pull requests.
To contribute, follow these steps:

1. Fork the repository on GitHub.
2. Clone your forked repository (`git clone https://github.com/ghaiith/bard-ai-telegram-bot.git`).
3. Create a new branch for your feature or bug fix (`git checkout -b new-feature`).
4. Make your changes and commit them (`git commit -m "Add new feature"`).
5. Push the changes to your forked repository (`git push origin new-feature`).
6. Open a pull request on the original repository and describe your changes in detail.

## Disclaimer

This project is a demonstration of integrating AI capabilities into a Telegram bot. The code is provided as-is, and any AI-generated content should be reviewed before being shared. Be aware of the ethical considerations and potential risks associated with AI-generated content.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

