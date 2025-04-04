# 🎓 AI Lecture Notes Generator

Transform lecture audio into structured, comprehensive notes using AI.

## Features

- 🎙️ Transcribes lecture audio using OpenAI's Whisper Large V3 model
- 📝 Generates well-structured markdown notes using Meta-Llama-3.1-8B
- 🧠 Identifies key concepts, points, and takeaways automatically
- 🚀 Simple web interface built with Gradio
- ⚡ Optimized with 4-bit quantization for efficient inference

## Demo



https://github.com/user-attachments/assets/eac0bcb7-dd5b-4ba0-8a82-2af5614e1da7



## How It Works

1. **Audio Transcription**: Converts lecture audio to text using Whisper Large V3
2. **Note Generation**: Processes transcription through Llama 3.1 to create structured notes
3. **Format Cleaning**: Ensures consistent markdown formatting with proper headers

## Installation

```bash
# Clone the repository
git clone https://github.com/Abdulllah-Rizwan/AI-Lecture-s-Note-Generator.git
cd AI-Lecture-s-Note-Generator

# Install dependencies
pip install -r requirements.txt
```

## Usage

### Option 1: Run the web interface

```python
python app.py
```

Then open your browser and navigate to the displayed URL (typically http://127.0.0.1:7860/).

### Option 2: Use the API programmatically

```python
from lecture_notes_generator import process_audio

# Generate notes from an audio file
notes = process_audio("path_to_lecture_audio.mp3")
print(notes)
```

## Requirements

- Python 3.8+
- PyTorch
- Transformers
- Gradio
- Hugging Face account with appropriate model access
- CUDA-compatible GPU (recommended)

## Output Format

The generated notes follow this structure:

```markdown
# Topic: [Lecture Topic]
## Instructor
[Instructor name if detected]
## Summary
[Concise summary of the lecture content]
## Key Concepts
- [Important concept 1]
- [Important concept 2]
...
## Key Points
- [Major point 1]
- [Major point 2]
...
## Takeaways
- [Takeaway 1]
- [Takeaway 2]
...
```

## Limitations

- Best suited for academic lectures with clear structure
- Audio quality significantly impacts transcription accuracy
- May require fine-tuning for specialized terminology

## License

MIT license

## Acknowledgements

- OpenAI for the Whisper model
- Meta for the Llama 3.1 model
- Hugging Face for model hosting and libraries
- Gradio for the web interface framework
