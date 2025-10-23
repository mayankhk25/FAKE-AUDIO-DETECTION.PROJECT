🧠 Synthetic-Voice-Detection-Vocoder-Artifacts
📁 LibriSeVoc Dataset
We are the first to identify neural vocoders as a source of features to expose synthetic human voices.
Here are the differences shown by the six vocoders compared to the original audio:

image

We provide LibriSeVoC as a dataset of self-vocoding samples created with six state-of-the-art vocoders to highlight and exploit the vocoder artifacts.
The composition of the dataset is shown in the following table:

image
The source of our dataset ground truth comes from LibriTTS. Therefore, we follow the naming logic of LibriTTS.
For example:
27_123349_000006_000000.wav →

27 is the reader's ID
123349 is the ID of the chapter
🎯 Deepfake Detection
We propose a new approach to detecting synthetic human voices by:

Exposing signal artifacts left by neural vocoders
Modifying and improving the RawNet2 baseline by adding multi-loss
✅ This lowers the error rate from 6.10% to 4.54% on the ASVspoof Dataset.

Here is the framework of the proposed synthesized voice detection method:

image
