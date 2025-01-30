# Malayalam-Audio-Translator
## Overview
Cascaded Speech-to-Speech translation model that translates audio input of some language into Malayalam. The project uses a cascaded pipeline approach for transcription, translation, and synthesis.

## Architecture
The model performs the following steps:

1. Transcription: Converts input audio to English text using OpenAI Whisper (openai/whisper-base) for automatic speech recognition (ASR).

2. Translation: Translates the transcribed English text into Malayalam using the multilingual text translation model facebook/mbart-large-50-many-to-many-mmt.

3. Synthesis: Converts the translated Malayalam text to speech using facebook/mms-tts-mal for text-to-speech synthesis.

## Dependencies

* transformers

* gradio

* datasets

* numpy

