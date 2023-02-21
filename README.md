# langchain-experiments
This repo contains Python code and Jupyter Colab notebooks to test various Langchain pipeline configurations.

## Experiment #1: Download YouTube audio, transcript, vectorize and query via similiarity search
STEPS:
a. Download YouTube audio as mp3 file
b. Transcript mp3 audio into timestamped text using OpenAI Whisper
c. Vectorize using OpenAI GPT-3 Vectorizer
d. Use Meta FAISS as store for vectorized transcript and questions
c. Use Langchain to coordinate cosine similiarity search to find nearest answer in transcript
Creation: 21 Feb 2023 @ 17:30EST
Last Run: (same)
