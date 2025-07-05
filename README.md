# Voice Extraction 

A Jupyter notebook for preparing audio datasets. This tool:

- Performs speaker diarization to separate speakers from a multi-speaker recording.

- Identifies the target speaker by comparing diarized segments against an isolated reference audio sample.

- Transcribes the selected audio snippets using Whisper and stores the results in a Hugging Face repository.

## Features

**Speaker Diarization**: Uses the pyannote pipeline to detect speaker turns and assign speaker IDs.

**Target Speaker Selection**: Computes embeddings for each diarized segment and a reference sample to identify the desired speaker.

**Transcription & Storage**: Leverages OpenAI Whisper for transcription and pushes the metadata and audio snippets to a Hugging Face Hub dataset.
