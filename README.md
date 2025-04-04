# 🎓 AI Lecture Notes Generator

Transform lecture audio into structured, comprehensive notes using AI.

## Features

- 🎙️ Transcribes lecture audio using OpenAI's Whisper Large V3 model
- 📝 Generates well-structured markdown notes using Meta-Llama-3.1-8B
- 🧠 Identifies key concepts, points, and takeaways automatically
- 🚀 Simple web interface built with Gradio
- ⚡ Optimized with 4-bit quantization for efficient inference

## Demo



https://github.com/user-attachments/assets/0f1fadb7-52ef-4be2-a866-d8085a37aa6d



## How It Works

1. **Audio Transcription**: Converts lecture audio to text using Whisper Large V3
2. **Note Generation**: Processes transcription through Llama 3.1 to create structured notes
3. **Format Cleaning**: Ensures consistent markdown formatting with proper headers

## Installation

```bash
# Clone the repository
git clone https://github.com/Abdulllah-Rizwan/AI_Lecture-s-Note-Generator.git
cd AI-Lecture-Notes-Generator

# Install dependencies
pip install requests torch bitsandbytes transformers sentencepiece accelerate gradio httpx==0.27.2
```

## Usage

### Option 1: Run the Jupyter Notebook

```bash
jupyter notebook "AI Lecture Notes Generator.ipynb"
```

Run all cells in the notebook to start the Gradio interface, then interact with the application through the displayed URL (typically http://127.0.0.1:7860/).

### Option 2: Use the functions directly in your code

You can import the functions from the notebook into your own Python code:

```python
# Import the necessary functions
from AI_Lecture_Notes_Generator import process_audio

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

MIT License.

## Acknowledgements

- OpenAI for the Whisper model
- Meta for the Llama 3.1 model
- Hugging Face for model hosting and libraries
- Gradio for the web interface framework
