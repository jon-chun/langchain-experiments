# langchain-experiments
This repo contains Python code and Jupyter Colab notebooks to test various Langchain pipeline configurations.


## Experiment #1: Download YouTube audio, transcript, vectorize and query via similiarity search

STEPS:

* Download YouTube audio as mp3 file
* Transcript mp3 audio into timestamped text using OpenAI Whisper
* Vectorize using OpenAI GPT-3 Vectorizer
* Use Meta FAISS as store for vectorized transcript and questions
* Use Langchain to coordinate cosine similiarity search to find nearest answer in transcript

Creation: 21 Feb 2023 @ 17:30EST
Last Run: (same)

---

YouTube title: "Steve Jobs' 2005 Stanford Commencement Address"
URL: https://www.youtube.com/watch?v=UF8uR6Z6KLc (15:04) 2008)

SAMPLE OUTPUT:

1. Q&A #1
* Question: How old was Steve Jobs when started Apple?
* Answer:  Steve Jobs was 20 when he started Apple.
* Sources: 00:05:47
2. Q&A #2
* Question: Where was Apple started?
* Answer:  Apple was started in Waz and Steve Jobs' parents' garage.
* Based on Time Stamp: 00:05:47, 00:05:51
3. Q&A #3
* Question: Who were the first employees of Apple?
* Answer:  The first employees of Apple were Steve Wozniak and Steve Jobs.
* Based on Time Stamp: 00:05:47, 00:05:51
4. Q&A #4
* Question: What makes a great entrepreneur?
* Answer:  A great entrepreneur has the courage to follow their heart and intuition.
* Based on Time Stamp: 00:12:46
5. Q&A #5
* Question: How do you deal with the fear of failure?
* Answer:  To deal with the fear of failure, have faith and believe that the dots will connect down the road, which will give you the confidence.
* Based on Time Stamp: 00:05:21, 00:08:16, 00:09:47
6. Q&A #6
* Question: What is the most important goal in life?
* Answer:  The most important goal in life is to have the courage to follow your heart and intuition.
* Based on Time Stamp: 00:12:46
7. Q&A #7
* Question: Do you fear failure?
* Answer:  I don't know.
* Based on Time Stamp: 00:09:47
8. Q&A #8
* Question: How do you deal with people who doubt you?
* Answer:  Don't lose faith and don't let the noise of others' opinions drown out your own inner voice.
* Based on Time Stamp: 00:08:16, 00:12:42
9. Q&A #9
* Question: What makes you happy?
* Answer:  Finding what you love makes you happy.
* Based on Time Stamp: 00:08:21, 00:08:27, 00:05:44
10. Q&A #10
* Question: Do you live with any regrets?
* Answer:  No, I do not live with any regrets.
* Based on Time Stamp: 00:12:13
11. Q&A #11
* Question: Do you have any regrets?
* Answer:  I do not know.
* Based on Time Stamp: 00:10:05, 00:01:45, 00:05:16, 00:12:13
