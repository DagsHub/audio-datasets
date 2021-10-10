# Voice Gender Detection 

## 1. General information

Cleaned Dataset for Voice gender detection using the VoxCeleb dataset (7000+ unique speakers and utterances, 3683 males / 2312 females). The VoxCeleb is an audio-visual dataset consisting of short clips of human speech, extracted from interview videos uploaded to YouTube. VoxCeleb contains speech from speakers spanning a wide range of different ethnicities, accents, professions and ages.

**The similar version of dataset is uploaded to [DagsHub](https://dagshub.com/kingabzpro/voice_gender_detection), enabling you to preview the dataset before downloading it.**

## 2. Data Preprocessing

The [author](https://github.com/jim-schwoebel) have downloaded all the files from [VoxCeleb2](http://www.robots.ox.ac.uk/~vgg/data/voxceleb/). After this, he cleaned the data to separate all the males from the females. I took one voice file at random for all the males and females so as to provide unique files.

![img](https://raw.githubusercontent.com/jim-schwoebel/voice_gender_detection/master/data/Screen%20Shot%202019-07-22%20at%2011.16.14%20AM.png)

To prepare the dataset, He put the 'males' and 'females' folders in the data directory of this repository. This will allow for us to featurize the files and train machine learning models via the provided training scripts.

![img](https://github.com/jim-schwoebel/gender-detection/raw/master/data/Screen%20Shot%202019-07-22%20at%2012.25.49%20PM.png)

## 3. Audio File Conversion

The [original files](https://drive.google.com/file/d/1HRbWocxwClGy9Fj1MQeugpR4vOaL9ebO/view) that I downloaded were in `.m4a` format which is not detectable by DAGsHub audio visualization, so I used [Python script to convert m4a files to wav files (github.com)](https://gist.github.com/arjunsharma97/0ecac61da2937ec52baf61af1aa1b759) to convert my dataset into `.wav` format. I ran code for the males and females folder separately. 

## 4. Organization of the dataset

The dataset is large (1.26GB) and simple to navigate as it has 2 folders based on binary gender. Males folder contains 3682 .wav audio files from unique speakers all over the world. Similar to the males folder we have females fold containing 2312 .wav files of unique females speakers. The audio duration range from 5~30 seconds to approximately 194 KB size. The following ASCII diagram depicts the directory structure.

```
<root directory>
    |
    .- README.md
    |
    .- fileconvert.py
    |
    .- females/
    |
    .- males/
          |
          .- 0.wav
          |
          .- 1.wav
          |
          .- 2.wav
          | ...

```

## 5. Use Case & Results

The dataset is used to train a machine learning model to detect males from females from audio files (90.7% +/- 1.3% accuracy). You can find more about code and results [here](https://github.com/jim-schwoebel/voice_gender_detection).

```python
Decision tree accuracy (+/-) 0.007327676542764603
0.7398596519424567
Gaussian NB accuracy (+/-) 0.016660391044338484
0.8682797740896762
SKlearn classifier accuracy (+/-) 0.00079538963465451
0.5157270607408913
Adaboost classifier accuracy (+/-) 0.013940745120583124
0.8892763651333413
Gradient boosting accuracy (+/-) 0.01950292233912751
0.8669747415791165
Logistic regression accuracy (+/-) 0.012678238150779661
0.894515837971657
Hard voting accuracy (+/-) 0.013226860908589952
0.9076178049591996
K Nearest Neighbors accuracy (+/-) 0.017244722910655787
0.731352177051436
Random forest accuracy (+/-) 0.02258623279374182
0.8079923672086033
svm accuracy (+/-) 0.022841304608332974
0.8781480823563248
most accurate classifier is Hard Voting with audio features (mfcc coefficients).
```

## Acknowledgments

First, I would like to thank Jim Schwoebel for publishing dataset on GitHub and explaining in depth how to use this dataset. Secondly, I would like to thank VoxCeleb for providing amazing open source dataset. 

*The VoxCeleb is supported by the EPSRC programme grant [Seebibyte EP/M013774/1: Visual Search for the Era of Big Data.](http://www.robots.ox.ac.uk/~vgg/projects/seebibyte/)*

## License

- The [VoxCeleb](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/) dataset is available to download for commercial/research purposes under a [Creative Commons Attribution 4.0 International License. ](https://creativecommons.org/licenses/by/4.0/) 
- Voice Gender Detection dataset is under [Apache License Version 2.0](http://www.apache.org/licenses/)  by Jim Schwoebel, 2020

---

Jim Schwoebel,
Aug 8, 2020

---

**Original Dataset**: [Voice Gender Detection ](https://drive.google.com/file/d/1HRbWocxwClGy9Fj1MQeugpR4vOaL9ebO/view)

**DAGsHub Dataset:** [kingabzpro/voice_gender_detection](https://dagshub.com/kingabzpro/voice_gender_detection)

------

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*
