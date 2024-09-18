
# Fourier Transform Animal Sound Analysis


This project performs an in-depth analysis of animal sounds, specifically focusing on cat and dog audio data. The key tool used is the Fourier Transform, which converts time-domain audio signals into their frequency components. This frequency-domain analysis reveals patterns in the audio data that are not immediately visible in the raw time-domain waveform.

The ultimate goal of this project is to visualize and classify distinct sound features, which can help in understanding and identifying the characteristics of different animal sounds. This analysis is done through a variety of signal processing techniques, using Fourier Transforms, along with other key audio features such as Mel-Frequency Cepstral Coefficients (MFCCs), zero-crossing rate, and chroma features.


## Project Overview
The analysis is performed using audio processing techniques implemented in Python, leveraging libraries like librosa for audio feature extraction. The notebook extracts features such as the Mel-Frequency Cepstral Coefficients (MFCCs), zero-crossing rate, chroma features, and more, which are commonly used in speech and audio signal processing. Visualizing these features helps in understanding the audio's characteristics, which can contribute to identifying the animal voice.

## Requirements
To run this project, you will need the following libraries:

- librosa: For audio processing and feature extraction.
- matplotlib: For visualizing the audio features.
- numpy: For numerical computations.
- google.colab (if running on Google Colab): For mounting Google Drive to access audio data..


## Steps Involved

#### 1. Environment Setup:

- Library Installation: The necessary Python packages such as librosa and numba are installed.
- Data Access: Audio files are loaded from Google Drive (or local storage), which can be used as input for feature extraction.

#### 2. Audio Loading and Visualization:
- Waveform Visualization: Audio files are loaded using librosa.load(). This converts the audio into a format that is ready for analysis, typically a NumPy array representing the amplitude of the sound over time.
- Time-Domain Visualization: The raw waveform of the audio is plotted to provide a basic visual understanding of the sound patterns. While this visualization is useful, it can be difficult to interpret complex sounds based purely on time-domain information.

#### 3. Feature Extraction:
- MFCCs (Mel-Frequency Cepstral Coefficients): MFCCs represent the short-term power spectrum of the audio. These are especially useful for identifying patterns in speech and animal sounds, as they mimic the human ear’s perception of sound frequencies.

- Zero Crossing Rate: This calculates how often the signal crosses the horizontal axis (i.e., changes from positive to negative or vice versa). It’s a useful metric for determining how "noisy" or "tonal" the audio is, which can help differentiate between the sharp sounds of barking versus the more continuous tones of a meow.

- Chroma Features: These are related to the harmonic content of the audio. They represent the pitch class of the sound and are particularly useful for analyzing sounds that have clear tonal structures (such as a meow or a howl).

- Spectrogram: A spectrogram is generated using the Short-Time Fourier Transform (STFT). It provides a visual representation of how the frequency content of the sound changes over time. This allows for identification of frequency bands where specific sounds, such as animal vocalizations, are more prominent.

#### 4. Fourier Transform Analysis:
- Fourier Transform is the cornerstone of this analysis. By converting the time-domain audio into frequency-domain data, we are able to decompose complex animal sounds into their individual frequency components.
- Spectral Analysis: By plotting the Fourier-transformed data, we can observe which frequencies are dominant in the sound, making it easier to differentiate between the sounds of cats and dogs.e

#### 5. Visualization:
- MFCC Visualization: MFCC coefficients are plotted to show the different spectral bands of the audio signal.
- Spectrogram Visualization: The spectrogram provides a frequency-over-time view, which allows us to see how the sound's frequency content evolves. This is useful for identifying dynamic changes, like a dog bark that starts at a low frequency and quickly shifts higher.

