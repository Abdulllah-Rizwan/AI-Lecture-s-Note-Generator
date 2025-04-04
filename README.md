🎓 AI Lecture Notes Generator
Transform lecture audio into structured, comprehensive notes using AI.
Features

🎙️ Transcribes lecture audio using OpenAI's Whisper Large V3 model
📝 Generates well-structured markdown notes using Meta-Llama-3.1-8B
🧠 Identifies key concepts, points, and takeaways automatically
🚀 Simple web interface built with Gradio
⚡ Optimized with 4-bit quantization for efficient inference

Demo

https://github.com/user-attachments/assets/433a8751-085b-4382-ba43-5c1e17be85c5




Audio Transcription: Converts lecture audio to text using Whisper Large V3
Note Generation: Processes transcription through Llama 3.1 to create structured notes
Format Cleaning: Ensures consistent markdown formatting with proper headers

Installation
bashCopy# Clone the repository
git clone https://github.com/yourusername/ai-lecture-notes-generator.git
cd ai-lecture-notes-generator

# Install dependencies
pip install -r requirements.txt
Usage
Option 1: Run the web interface
pythonCopypython app.py
Then open your browser and navigate to the displayed URL (typically http://127.0.0.1:7860/).
Option 2: Use the API programmatically
pythonCopyfrom lecture_notes_generator import process_audio

# Generate notes from an audio file
notes = process_audio("path_to_lecture_audio.mp3")
print(notes)
Requirements

Python 3.8+
PyTorch
Transformers
Gradio
Hugging Face account with appropriate model access
CUDA-compatible GPU (recommended)

Output Format
The generated notes follow this structure:
markdownCopy# Topic: [Lecture Topic]
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
Limitations

Best suited for academic lectures with clear structure
Audio quality significantly impacts transcription accuracy
May require fine-tuning for specialized terminology

License
[Your License] 

Acknowledgements

OpenAI for the Whisper model
Meta for the Llama 3.1 model
Hugging Face for model hosting and libraries
Gradio for the web interface framework
