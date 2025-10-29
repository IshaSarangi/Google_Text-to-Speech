# Google_Text-to-Speech
Scenario:
Imagine you are working for a digital publishing company that wants to develop a smart audiobook assistant. This assistant should be able to:
- Transcribe voice narration from long-form audiobook recordings.
- Detect transcription mismatches or errors in the recordings for quality assurance (QA).
- Enable text-to-speech feedback for quick corrections or previews.
- Evaluate narration fidelity, particularly if AI-based narrators are used.

Objectives:
Audio upload simulate a folder names wavs/ with audio files (e.g., LJ001-0001.wav). Use the filename and transcript mapping from metadata_df_pipe.
Speech Recognition (ASR) using Whisper Load audio from wavs/dictionary. Use Whisper to transcribe and compare it with ground truth from metadata.
Add background noise (Challenge Simulation), mix the audio with cafe background noise using pydub.
Text-to-Speech (TTS) response generate a simple response like: "Your order of cappuccino has been received." Use gTTS or pyttsx3 to convert this text to audio.
