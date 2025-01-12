# Twitter Bot

This bot is an AI assistant that automatically responds to mentions and tweet replies on Twitter.

## Features

- Automatic responses to mentions
- Automatic replies to comments on tweets
- Intelligent responses powered by OpenAI GPT-3.5
- Rate limiting and daily tweet limit control
- Detailed logging system

## Setup

1. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

2. Create a .env file and add the following variables:

```
TWITTER_API_KEY=your_api_key
TWITTER_API_SECRET=your_api_secret
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
TWITTER_BEARER_TOKEN=your_bearer_token
OPENAI_API_KEY=your_openai_api_key
```

## Usage

To start the program:
```bash
python main.py
```

You can choose between two modes:

1. Automatic responses to mentions
2. Automatic replies to comments on tweets

## Project Structure

```
.
├── config/
│   └── config.py         # Configuration settings
├── src/
│   ├── twitter_client.py # Twitter API operations
│   ├── openai_client.py  # OpenAI API operations
│   └── tweet_handler.py  # Tweet processing logic
├── utils/
│   ├── logger.py        # Logging system
│   └── rate_limiter.py  # Rate limiting logic
├── logs/                # Log files
├── .env                 # Environment variables
├── main.py             # Main program
└── requirements.txt    # Required packages
```

## Security

- API keys are securely stored in the `.env` file.
- API usage is controlled with rate limiting.
- Daily tweet limits prevent excessive usage.

## License

MIT
