# Poetry Duel Arena

A Gradio-based application where AI poets with distinct personas compete to create poetry based on an uploaded document. An AI judge evaluates the verses, and the winning lines form a collaborative poem. Features include text extraction from PDF, DOCX, TXT, and images, and audio generation of the final poem.

## Features
- **AI Poets**: Six personas (Romantic, Modernist, Classical, Haiku, Surrealist, Beat) with unique styles.
- **Document Processing**: Supports PDF, DOCX, TXT, and image files (via OCR).
- **Judging System**: Evaluates verses on factual grounding, poetic quality, coherence, originality, and emotional impact.
- **Audio Output**: Generates an MP3 of the final poem using Google Text-to-Speech.

## Setup for Hugging Face Spaces

1. **Create a Hugging Face Space**:
   - Go to [Hugging Face Spaces](https://huggingface.co/spaces).
   - Create a new Space, select "Gradio" as the SDK, and choose "Python" as the template.
   - Clone this repository into the Space.

2. **Install Dependencies**:
   - Ensure `requirements.txt` and `apt.txt` are in the root directory.
   - Hugging Face will automatically install Python dependencies from `requirements.txt` and system packages from `apt.txt`.

3. **Set Up Environment Variables**:
   - Add your `OPENAI_API_KEY` in the Space settings under "Repository Secrets":
     - Go to Space Settings > Repository Secrets > New Secret.
     - Name: `OPENAI_API_KEY`.
     - Value: Your OpenAI API key.

4. **Run the App**:
   - The app will run automatically on Hugging Face Spaces using `app.py`.
   - Access the Gradio interface via the provided Space URL.

## Local Development

### Prerequisites
- Python 3.8+
- System dependencies: `tesseract-ocr`, `tesseract-ocr-eng`, `poppler-utils`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/poetry-duel.git
   cd poetry-duel