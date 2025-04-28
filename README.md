# Discord Bot

## Overview

A simple Discord bot built with Python and `discord.py` that can:

- Welcome new members
- Respond to commands
- Assign and remove a special role ("Gamer")
- Filter out bad language
- Create polls
- Handle secret commands restricted to specific roles

## Features

### Welcome Message
- Automatically sends a private welcome message to users when they join the server.

### Bad Word Filter
- Deletes messages containing banned words (e.g., "shit") and warns the user.

### Commands
- `!hello`: Replies with a greeting.
- `!assign`: Assigns the "Gamer" role to the user.
- `!remove`: Removes the "Gamer" role from the user.
- `!dm <message>`: Sends a private DM to the user with their message.
- `!reply <message>`: Replies to the user's message publicly.
- `!poll <question>`: Creates a poll with thumbs up/down reactions.
- `!secret`: Restricted command only accessible to users with the "Gamer" role.

### Error Handling
- Users without the "Gamer" role receive a permission error if they try to access secret commands.

### Logging
- All bot activity is logged in `discord.log`.

## Setup

### Clone the repository
```bash
git clone https://github.com/yourusername/your-bot-repo.git
cd your-bot-repo
```

### Install the dependencies

```bash
pip install discord.py python-dotenv
```
Create a .env file
- Inside the project folder, create a .env file and add your Discord bot token: