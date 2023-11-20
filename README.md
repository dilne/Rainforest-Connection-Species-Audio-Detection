<h1 align="center">🦜Rainforest Connection Species Audio Detection🐸</h1>

[Notebook](https://github.com/dilne/Rainforest-Connection-Species-Audio-Detection/blob/main/Notebook.ipynb)

<a href="https://colab.research.google.com/github/dilneRainforest-Connection-Species-Audio-Detection/blob/main/Notebook.ipynb" target="_blank">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## Summary
A modified ResNet18 model is used to predict the species from 24 types. After trimming the audio samples from the dataset to the correct length to match the species' call and implementing a band pass filter to remove the frequencies outiside the range of the call, the highest validation accuracy achieved was 0.72, but there are certainly ways to improve this model, including introducing other data preprocessing techniques.

The dataset can be found from [the official Kaggle page](https://www.kaggle.com/competitions/rfcx-species-audio-detection/).

## Future Steps for Preprocessing the Dataset
- <b>Pitch shift:</b> Pitch shifting all the audio to have an equal centre frequency could improve generalisation
- <b>Set dB level:</b> Making the data the same dB level (maybe having equal RMS?), could encourage the model to infer mainly from frequency data
