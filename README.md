# llm-coding-challenge
This is a submission to LLM coding challenge from CloudWalk.io

Used MFCC preprocessing and Fast Fourier Transform to extract features from audio files.

Since the audio features are sequential, Bidirectional LSTM is an appropriate model type. This model type is sensitive to features at the start of audio and the end of the audio. 
Two layers of LSTM were sufficient enough to reach a high precision rate.

The performance is measured using F1 scores to ensure that the model is measured accurately.
CrossEntropy loss and Adam optimizer is used for model training.

During the preprocessing, white noise were added to make the data more resilient.

The final model acheived 98.67% precision.