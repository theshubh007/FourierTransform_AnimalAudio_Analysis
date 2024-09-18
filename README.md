
# Fourier Transform Animal Sound Analysis


This project performs an analysis of animal sounds (cats and dogs) using Fourier Transforms to convert time-domain audio signals into their frequency components. The goal is to visualize and classify different sound features.


## Project Overview
The analysis is performed using audio processing techniques implemented in Python, leveraging libraries like librosa for audio feature extraction. The notebook extracts features such as the Mel-Frequency Cepstral Coefficients (MFCCs), zero-crossing rate, chroma features, and more, which are commonly used in speech and audio signal processing. Visualizing these features helps in understanding the audio's characteristics, which can contribute to identifying the animal voice.

## Requirements
To run this project, you will need the following libraries:

- librosa: For audio processing and feature extraction.
- matplotlib: For visualizing the audio features.
- numpy: For numerical computations.
- google.colab (if running on Google Colab): For mounting Google Drive to access audio data..


## Steps Involved

#### Environment Setup:

- The notebook installs required libraries (librosa, numba) and mounts Google Drive to access audio files stored there.

#### Audio Loading and Visualization:
- Audio files are loaded using librosa.load(), and the waveform of the audio is displayed to visualize the sound patterns.

#### Feature Extraction:
- MFCCs (Mel-Frequency Cepstral Coefficients): Extracts the coefficients that represent the short-term power spectrum of the audio.
- Zero Crossing Rate: Calculates the rate at which the signal changes sign, helping to measure the noisiness of the audio.
- Chroma Features: Used to represent the harmonic and pitch content of the audio.
- Spectrogram: A visual representation of the spectrum of frequencies as they vary over time.

#### Visualization:
- The extracted features are plotted using matplotlib to provide insights into the audio's characteristics.
- These visualizations can assist in identifying the sound of animals, which can be helpful in varios commenrcial usecases like
