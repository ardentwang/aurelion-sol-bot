Aurelion Sol Discord bot written in Python that uses the [completions API](https://beta.openai.com/docs/api-reference/completions) to have conversations with the `text-davinci-003` model, and the [moderations API](https://beta.openai.com/docs/api-reference/moderations) to filter the messages.

This bot uses the [OpenAI Python Library](https://github.com/openai/openai-python) and [discord.py](https://discordpy.readthedocs.io/).

# Features

- `/chat` starts a public thread, with a `message` argument which is the first user message passed to the bot
- The model will generate a reply for every user message in any threads started with `/chat`
- The entire thread will be passed to the model for each request, so the model will remember previous messages in the thread

# FAQ

> Why isn't my bot responding to commands?

Ensure that the channels your bots have access to allow the bot to have these permissions.
- Send Messages
- Send Messages in Threads
- Create Public Threads
- Manage Messages (only for moderation to delete blocked messages)
- Manage Threads
- Read Message History
- Use Application Commands
