# Video-Ppt-Pdf-Transcription-
This project automates the process of generating structured lecture notes by combining audio transcriptions from lecture videos with slide content and speaker notes from PowerPoint presentations. The final output is a comprehensive and well-formatted PDF containing all relevant lecture information.

Features
Converts .mkv lecture videos to .mp4

Extracts audio (.wav) for Whisper compatibility

Transcribes audio using OpenAI’s Whisper ASR model

Parses .pptx files to extract:

Slide titles

Slide text content

Slide speaker notes

Merges transcriptions and slide content into a readable PDF


Pipeline Overview
MKV to MP4 Conversion
Converts lecture videos from .mkv to .mp4 using ffmpeg for better compatibility.

Audio Extraction
Extracts .wav audio from the .mp4 file to be used for transcription.

Transcription with Whisper
Uses OpenAI’s Whisper model (medium or large) to convert spoken audio into accurate text.

PPT Content Extraction
Parses .pptx slides to collect:

Slide title

Text content (bullet points or descriptions)

Speaker notes

PDF Generation
Combines the full transcript and extracted slide content into a clean, structured PDF using the fpdf library.


Requirements
ffmpeg-python
openai-whisper
python-pptx
fpdf
