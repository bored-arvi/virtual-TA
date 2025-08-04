# Virtual TA (Teaching Assistant)

Virtual TA is a Python-based project designed to assist with course content embedding, document conversion, and AI-powered educational tools.

## Features
- **Document Processing**: Converts course content (PDFs, Markdown, etc.) into embeddings for semantic search.
- **Embeddings & AI**: Uses machine learning models to embed and analyze course data.
- **Content Cleaning**: Includes utilities for cleaning and preparing datasets.
- **Docker Support**: Containerized environment for easy deployment.

## Quick Installation
For detailed instructions, check [INSTALLATION.md](INSTALLATION.md).

### Basic Steps
```bash
git clone https://github.com/your-username/virtual-TA.git
cd virtual-TA
python -m venv venv
venv\Scripts\activate  # Windows
# or
source venv/bin/activate # macOS/Linux
pip install -r requirements.txt
```

## Usage
Run the main program:
```bash
python main.py
```

## Project Structure
- `main.py` – Main entry point of the application.
- `embedder.py` – Embedding generation logic.
- `cleaner.py` – Data cleaning and preprocessing utilities.
- `markdown_converter.py` – Convert markdown content.
- `course_md/` – Course material in Markdown format.
- `tds_docs.db` – Sample SQLite database.
- `requirements.txt` – Python dependencies.

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
