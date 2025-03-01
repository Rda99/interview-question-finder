# AI-Powered Interview Question Finder

This tool automatically finds and presents relevant interview questions based on company name and job role, using AI to extract questions from web content.

## Features

- Search for interview questions with just company name and job role
- AI-powered extraction of relevant questions from web content
- Clean, responsive UI for easy viewing of results
- Database storage for quick retrieval of previously found questions

## Architecture

```
User Input --> Search Query Generator --> Web Scraper --> Content Extractor
    --> Question Classifier --> Database --> Recommendation Engine --> User Interface
```

## Installation

1. Clone this repository
```bash
git clone https://github.com/yourusername/interview-question-finder.git
cd interview-question-finder
```

2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Set up environment variables
```bash
cp .env.example .env
# Edit .env to add your OpenAI API key
```

5. Run the application
```bash
python app.py
```

The application will be available at http://127.0.0.1:5000/

## Usage

1. Enter a company name (e.g., "Google")
2. Enter a job role (e.g., "Software Engineer")
3. Click "Find Questions"
4. View the results organized by source

## Technical Details

- **Backend**: Python with Flask
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite
- **AI**: OpenAI GPT for question extraction
- **Web Scraping**: BeautifulSoup4

## Legal Considerations

This tool is for educational purposes only. Be sure to:
- Respect website terms of service and robots.txt directives
- Implement rate limiting for web scraping
- Give proper attribution to sources
- Use the information ethically

## Future Improvements

- Add user accounts for saving favorite questions
- Implement caching to reduce API calls
- Add question categorization (technical, behavioral, etc.)
- Improve search relevance with ML algorithms

## License

MIT
