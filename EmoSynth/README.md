# EmoSynth: The Emotional Synthetic Audio Dataset

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3727593.svg)](https://doi.org/10.5281/zenodo.3727593)

## 1. General information

The ability of sound to enhance human wellbeing has been known since ancient civilizations, and methods can be found today across domains of health and within a variety of cultures. 
![image](https://dagshub.com/kingabzpro/EmoSynth/raw/master/assets/image.jpg)
**EmoSynth** is a dataset of 144 audio files which have been labelled by 40 listeners for their the perceived emotion, in regards to the dimensions of Valence and Arousal. 

**The similar version of dataset is uploaded to DagsHub: [EmoSynth](https://dagshub.com/kingabzpro/EmoSynth) , enabling you to preview the dataset before downloading it.**

## 2. Organization of the dataset

The dataset is small (106MB) and simple to navigate as it has only one folder based containing synthetic audio files. We also have an `audio_labels.csv` file, which contains details about the classification of audio based on the dimensions of Valence and Arousal. Each audio file is approximate 5 seconds long and 430 KB in size. 

*For the best experience keep your volume high to listen to the sounds.*

```
<root directory>
    |
    .- README.md
    |
    .- meta.txt
    |
    .- citation.txt
    |
    .- audio_labels.csv
    |
    .- Audio-Data/
          |
          .- s1_a0_d1.wav
          |
          .- s1_a0_d2.wav
          |
          .- s1_a1_d1.wav
          | ...
```

- **meta.txt**: contains labeling collection information.
- **citation.txt**: contains citation data for research paper.
- **audio_labels.csv**: contains labels of audio based on perceived listener rating form 1-5. 
  - audio_file: wav audio files name
  - valence: average rating of valence (1~5)
  - arousal: average rating of arousal (1~5)
  - round_val: round valence mean rating
  - round_ar: round arousal mean rating
  - round_val_sd: round valence standard deviation 
  - round_ar_sd: round arousal standard deviation 

## 3. Results

Results on the dataset show that Arousal does correlate moderately to fundamental frequency, and that the sine waveform is perceived as significantly different to square and sawtooth waveforms when evaluating perceived Arousal. The general results suggest that isolated synthetic audio can be modelled as a means of evoking affective states of emotion.

## Acknowledgments

First, I would like to thank Baird, Alice and Parada-Cabaleiro, Emilia and Fraser, Cameron and Hantke, Simone and Schuller, Bjorn for publishing dataset on Zendo and explaining the results. Secondly, I would like to thank Zenodo for maintaining amazing open source dataset.

------

Alice Baird; Emilia Parada-Cabaleiro, Aug 20, 2019

---

**Original Dataset**: [EmoSynth| Zenodo](https://zenodo.org/record/3727593#.YWAzaWJBzIV)

**DAGsHub Dataset:** [kingabzpro/EmoSynth](https://dagshub.com/kingabzpro/EmoSynth)

**Photo** by [Jonathan Borba](https://unsplash.com/@jonathanborba?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/romance?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

---
*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*

