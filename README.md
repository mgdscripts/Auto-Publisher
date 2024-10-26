
# Discord Auto-Publish Bot

This bot automatically publishes messages to announcement channels in a specified Discord server. Designed for use with announcement channels, it listens for messages and publishes them using the Discord API.

## Features

- **Auto-Publish Messages**: Publishes messages automatically in the specified announcement channel.
- **Status Notifications**: Logs success or failure of the publish action.

## Setup Instructions

### Prerequisites

- Python 3.8+
- [discord.py](https://github.com/Rapptz/discord.py) library (ensure it’s compatible with your Python version)
- `requests` library

### Installation

1. Clone the repository or download the source code.
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

### Configuration

1. Set your **bot token** in the `TOKEN` variable.
2. Update the `CHANNEL_ID` and `SERVER_ID` with your specific Discord channel and server IDs.

### Usage

1. Run the bot:
   ```bash
   python bot.py
   ```
2. The bot will listen for messages in the specified channel and automatically publish them.

### Code Explanation

- **Event Handlers**:
  - `on_ready`: Notifies when the bot is logged in.
  - `on_message`: Listens for messages in the specified `CHANNEL_ID` and triggers `publish_message`.
- **Helper Function**:
  - `publish_message`: Uses the Discord API to publish messages in announcement channels.

### Example Configuration

Replace placeholders with actual values:
```python
TOKEN = 'YOUR_BOT_TOKEN'
CHANNEL_ID = 123456789012345678  # Announcement channel ID
SERVER_ID = 123456789012345678  # Server ID
```

### Additional Notes

- Ensure the bot has the necessary permissions to manage and publish messages in the specified channel.
- The bot uses Discord's v9 API for message cross-posting; ensure your token and permissions allow API access.

---

This bot was created for automated announcement management in Discord servers.
