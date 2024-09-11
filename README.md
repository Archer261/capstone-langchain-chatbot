# ArcherBot: Your AI Assistant for Precision and Knowledge on Diet and Nutrition

ArcherBot is an intelligent chatbot application built with Flask and powered by the Cohere AI platform. It utilizes a knowledge base derived from "Encyclopedia of Diet: A Treatise on the Food Question, Vol. 5 of 5" to provide accurate and context-aware responses to user queries about diet and nutrition.

Created by Joseph Archer

## Features

- Interactive chat interface
- Multiple response modes:
  - Answer as Chatbot
  - Answer from Knowledge Base
  - Search Knowledge Base
- Powered by Cohere's language model
- Utilizes LangChain for enhanced conversational abilities
- Responsive design using Bootstrap
- Knowledge base sourced from "Encyclopedia of Diet: A Treatise on the Food Question, Vol. 5 of 5"

## Knowledge Base

The ArcherBot's responses are based on information from "Encyclopedia of Diet: A Treatise on the Food Question, Vol. 5 of 5". This comprehensive resource provides a wealth of information on diet, nutrition, and food-related topics. Users can expect responses that reflect the knowledge and perspectives presented in this encyclopedia.

Please note:
- The information provided is based on the content of the encyclopedia and may not reflect the most current nutritional science.
- For up-to-date medical or nutritional advice, always consult with a qualified healthcare professional.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7+
- pip (Python package manager)
- A Cohere API key (sign up at [cohere.ai](https://cohere.ai) if you don't have one)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/josepharcher/archerbot.git
   cd archerbot
   ```

2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root directory and add your Cohere API key:
   ```
   COHERE_API_KEY=your_actual_api_key_here
   ```

## Usage

1. Start the Flask development server:
   ```
   python app.py
   ```

2. Open a web browser and navigate to `http://localhost:5000`

3. Use the chat interface to interact with ArcherBot:
   - Select the desired response mode from the dropdown menu
   - Type your message in the input field
   - Click the send button or press Enter to submit your query

4. To clear the chat history, click the trash icon button

## Project Structure

- `app.py`: Main Flask application file
- `templates/index.html`: HTML template for the chat interface
- `static/main.js`: JavaScript file for handling chat functionality
- `static/style.css`: CSS file for additional styling (if any)
- `requirements.txt`: List of Python dependencies
- `.env`: Configuration file for environment variables (not tracked in git)
- `db/`: Directory containing the knowledge base derived from the Encyclopedia of Diet

## Customization

### Changing the Color Scheme

The current design uses a purple and red color scheme. To modify this:

1. Open `templates/index.html`
2. Locate the `<style>` section
3. Update the color values as desired

### Modifying the Knowledge Base

The current knowledge base is derived from "Encyclopedia of Diet: A Treatise on the Food Question, Vol. 5 of 5". If you wish to update or replace the knowledge base:

1. Ensure your new knowledge base is compatible with the Chroma vector store
2. Update the `db` directory with your new knowledge base files
3. Modify the `load_db()` function in `app.py` if necessary to accommodate any structural changes
4. Update this README to reflect the new source of information

## Troubleshooting

If you encounter any issues:

1. Ensure all dependencies are correctly installed
2. Verify that your `.env` file contains the correct Cohere API key
3. Check the console for any error messages
4. Make sure you're using a compatible Python version

## Contributing

Contributions to ArcherBot are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- [Flask](https://flask.palletsprojects.com/)
- [Cohere](https://cohere.ai/)
- [LangChain](https://github.com/hwchase17/langchain)
- [Bootstrap](https://getbootstrap.com/)
- "Encyclopedia of Diet: A Treatise on the Food Question, Vol. 5 of 5" for providing the knowledge base

## Author

Joseph Archer

For questions or feedback, please contact Joseph Archer at [your-email@example.com].