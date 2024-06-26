
# QuickVoiceBot

QuickVoiceBot is an AI-powered conversational voice bot that utilizes streaming speech-to-text, text-to-speech, and a large language model to engage in fast, fluid conversations. It provides a seamless voice interface for natural interactions.

## Features

- Real-time speech recognition using Deepgram's streaming API
- Natural-sounding text-to-speech powered by Deepgram
- Intelligent responses generated by a powerful language model (Groq or OpenAI)
- Streaming capabilities for fast, low-latency interactions
- Simple, easy-to-use conversation flow

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/QuickVoiceBot.git
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up your API keys:
   - Sign up for a Deepgram account and obtain an API key
   - (Optional) Sign up for an OpenAI account and obtain an API key if using OpenAI's models
   - Create a `.env` file in the project root and add your API keys:
     ```
     DEEPGRAM_API_KEY=your_deepgram_api_key
     OPENAI_API_KEY=your_openai_api_key
     ```

4. Run the bot:
   ```
   python main.py
   ```

## Usage

1. Start the bot by running `main.py`
2. Speak to the bot and it will respond with voice
3. Say "goodbye" to end the conversation

## Customization

- Adjust the language model settings in `main.py`:
  - Choose between Groq and OpenAI models by uncommenting the appropriate lines
  - Modify the model names and parameters as needed
- Customize the system prompt in `system_prompt.txt` to define the bot's persona and behavior
- Experiment with different Deepgram models for speech recognition and synthesis

## File Structure

- `main.py`: Main entry point of the application
- `system_prompt.txt`: File containing the system prompt for the language model
- `requirements.txt`: List of required Python packages
- `building_blocks/`: Directory containing isolated components for inspection
  - `speech_to_text_streaming.py`: Standalone example of streaming speech recognition
  - `text_to_speech.py`: Standalone example of text-to-speech
  - `llm.py`: Standalone example of using the language model

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- [Deepgram](https://deepgram.com/) for providing the speech recognition and synthesis APIs
- [Groq](https://groq.com/) for the powerful language model
- [OpenAI](https://openai.com/) for the alternative language model option
