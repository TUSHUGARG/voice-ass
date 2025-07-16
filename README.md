# Voice Virtual Assistant Using ElevenLabs API

## Overview

This project demonstrates how to build a professional Voice Virtual Assistant leveraging the ElevenLabs Conversational AI API and Python. The assistant supports real-time voice and text interactions, providing a seamless and context-aware conversational experience.

## Author

Tushar Garg

## Prerequisites

- Python 3.7 or higher
- ElevenLabs API credentials (AGENT_ID and API_KEY)
- Python packages:
  - `python-dotenv`
  - `elevenlabs`
  - `elevenlabs[pyaudio]` (for audio support)

## Setup Instructions

1. **Clone the repository** or download the project files.

2. **Create a `.env` file** in the project root directory with the following content:

   ```
   AGENT_ID=your_agent_id_here
   API_KEY=your_api_key_here
   ```

3. **Install dependencies** using pip:

   ```bash
   pip install python-dotenv elevenlabs elevenlabs[pyaudio]
   ```

4. **(Optional) Install system dependencies for audio:**

   - On Linux:

     ```bash
     sudo apt install portaudio19
     ```

   - On macOS:

     ```bash
     brew install portaudio
     ```

## Usage

Run the voice assistant script:

```bash
python voice_ass.py
```

The assistant will greet you and await your input. You can interact by typing messages in the console. To exit the session, type `exit` or `quit`.

## Code Highlights

- **Environment Configuration:** Securely loads API credentials from `.env` using `python-dotenv`.
- **Conversation Setup:** Configures the assistant with a personalized prompt and initial greeting.
- **Callbacks:** Implements callbacks to handle and display agent responses, interruptions, and user transcripts.
- **Interactive Loop:** Accepts user text input, sends it to the assistant, and outputs responses in real time.
- **Graceful Termination:** Supports exit commands and keyboard interrupt handling.

## Customization

- Modify the `user_name` and `schedule` variables in `voice_ass.py` to tailor the assistant’s context.
- Adjust the prompt and first message in the conversation configuration to suit your use case.

## Troubleshooting

- Verify that your `.env` file contains valid and correctly formatted API credentials.
- Ensure all Python dependencies are installed.
- Confirm audio devices are properly configured if using voice features.

## Additional Resources

- [ElevenLabs Conversational AI Documentation](https://elevenlabs.io/docs/conversational-ai/overview)
- [ElevenLabs Python SDK](https://elevenlabs.io/docs/conversational-ai/libraries/python)
- [Client Tools for Customization](https://elevenlabs.io/docs/conversational-ai/customization/tools-events/client-tools)
- [Retrieval-Augmented Generation (RAG)](https://elevenlabs.io/docs/conversational-ai/customization/knowledge-base/rag)

## License

This project is provided "as-is" without warranties. Use at your own discretion.

---

For further assistance or inquiries, please contact the project maintainer.
