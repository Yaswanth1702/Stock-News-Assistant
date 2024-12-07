# Stock News Assistant

**Stock News Assistant** is an interactive Python application designed to keep you informed about the latest news of publicly traded companies. Leveraging voice recognition, natural language processing, and text-to-speech technologies, it provides a seamless, hands-free way to fetch, summarize, and listen to news articles about stock tickers. It also features voice cloning, allowing a personalized and unique user experience.

## Features

- **Voice Interaction**: Speak to the assistant to provide company names, and it responds with relevant news summaries.
- **Ticker Recognition**: Matches spoken company names with S&P 500 and NASDAQ-100 stock tickers.
- **Real-Time News Aggregation**: Retrieves up-to-date news articles from the [Alpha Vantage API](https://www.alphavantage.co/).
- **Summarized Insights**: Uses advanced NLP models from Hugging Face to summarize lengthy articles into concise and meaningful information.
- **Text-to-Speech Conversion**: Reads news summaries aloud using customizable voices through the [Coqui TTS API](https://github.com/coqui-ai/TTS).
- **Voice Cloning**: 
  - Supports personalized voice synthesis by cloning a user's or preferred speaker's voice from a 6-second audio clip.
  - Allows users to configure the assistant to read out summaries in their own voice or another speaker's voice for a unique and engaging experience.
- **Interactive Commands**: Responds to user commands like "exit" to quit the application or continue fetching news for other companies.

## Usage

1. **Run the Assistant**:
   ```bash
   python stock_news_assistant.py
   ```
2. **Interact with the Assistant**:
   - Speak the name of a company (e.g., "Apple") when prompted.
   - The assistant identifies the stock ticker and retrieves the latest news.
   - Hear summaries of the top news articles.
   - If voice cloning is configured, the assistant reads out news summaries in the cloned voice.
   - Continue querying for other companies or say "exit" to quit.

## Example Interaction
- **Assistant**: "Please speak the company name."
- **User**: "Microsoft"
- **Assistant**: "Fetching news for MSFT..."
- **Assistant**: *Reads out the summarized news articles in the user-configured cloned voice.*

## Technologies Used

- **Natural Language Processing**:
  - Hugging Face `transformers` for article summarization.
  - `NLTK` for tokenization and text preprocessing.

- **Voice Interaction**:
  - `speech_recognition` for capturing and processing user voice input.
  - [Coqui TTS](https://github.com/coqui-ai/TTS) for synthesizing spoken output.
  - Voice cloning for personalized text-to-speech experiences.

- **Web Scraping and Data Handling**:
  - `BeautifulSoup` for extracting article content.
  - `pandas` for processing stock ticker data.

- **News Retrieval**:
  - Integrated with [Alpha Vantage API](https://www.alphavantage.co/).

Experience the future of stock news updates with personalized voice cloning and intelligent summarization.
