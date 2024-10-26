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
