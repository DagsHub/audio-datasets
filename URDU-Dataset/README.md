# URDU-Dataset
![banner](https://dagshub.com/kingabzpro/URDU-Dataset/raw/master/asset/urdu-dataset-banner.jpg)

## 1. General information

The URDU dataset contains emotional utterances of Urdu speech gathered from Urdu talk shows. There are 400 utterances of four basic emotions in the book: Angry, Happy, Neutral, and Emotion. There are 38 speakers (27 male and 11 female). This data is created from YouTube. Speakers are randomly selected.

**The similar version of dataset is uploaded to DagsHub: [URDU-Dataset](https://dagshub.com/kingabzpro/URDU-Dataset), enabling you to preview the dataset before downloading it.**

## 2. Structure

Nomenclature followed while naming the files in the dataset is to provide information about the speaker, gender, number of the file for that speaker, and overall numbering of the file in a particular emotion. Files are named as follows:

General Name: SGX_FXX_EYY

For more details about the dataset, please refer to the complete paper "Cross Lingual Speech Emotion Recognition: Urdu vs. Western Languages". https://arxiv.org/pdf/1812.10411.pdf

### 2.1 Audio files:

* [21M] Angry - of approximately 242 seconds of "clean" speech in `.wav` format **(pushed to DagsHub)**
 
* [21M] Happy - of approximately 244 seconds of "clean" speech `.wav` format **(pushed to DagsHub)**
 
* [21M] Neutral - of approximately 244 seconds of "clean" speech `.wav` format **(pushed to DagsHub)**

* [21M] Sad - of approximately 244 seconds of "clean" speech `.wav` format **(pushed to DagsHub)**

### 2.2 Organization of the Emotions dataset

The dataset is small (88MB) and simple to navigate as it has 4 folders based on emotions. Each folder contains 100 `.wav` audio files containing the emotions of Urdu speakers. The audio file range from 2~3 second of audio taken from a various video uploaded on YouTube. A representation of the directory structure can be seen in the ASCII diagram below.

```
<root directory>
    |
    .- README.md
    |
    .- Angry/
    |
    .- Happy/
    |
    .- Neutral/
    |
    .- Sad/
          |
          .- SF10_F1_S01.wav
          |
          .- SF10_F2_S02.wav  
          | ...

```

The name of audio file can be divided into three segments which is segregated by underscore(_) sign.

Where,

- In SGX, G indicates the gender of the speaker, which can be M for male speaker and F for female speaker, while X represents the speaker ID which remains the same for a particular speaker in all the emotions.

- In FXX, F is a keyword presenting file and XX indicates the number of files for a particular speaker.

- In EYY, E provides the information about emotion i.e., A, H, N, and S for Angry, Happy, Neutral, and Sad. respectively.

For example, file name SM1_F01_A12 indicates that this is 1st file recorded by speaker No. 1 and A12 indicates that this is the 12th file of Angry emotion.

## 3. Use Case

Cross lingual speech emotion recognition is an important task for practical applications. The performance of automatic speech emotion recognition systems degrades in cross-corpus scenarios, particularly in scenarios involving multiple languages or a previously unseen language such as Urdu for which limited or no data is available.

## 4. Results

The data of multiple languages are used for training. Results for emotion detection are increased even for the URDU dataset, which is highly dissimilar from other databases. Also, accuracy is boosted when a small fraction of testing data is included in the training of the model with a single corpus. These findings would be very helpful for designing robust emotion recognition systems even for languages having limited or no dataset. [Cross Lingual Speech Emotion Recognition: Urdu vs. Western Languages](https://arxiv.org/pdf/1812.10411.pdf)

## Acknowledgments

First and foremost, I would like to thank Siddique Latif and his team from *Information Technology University (ITU)-Punjab* and *COMSATS University Islamabad (CUI), Islamabad* for pushing the audio dataset to GitHub. 

We would like to thank Farwa Anees, Muhammad Usman, Muhammad Atif, and Farid Ullah Khan for assisting us in the preparation of the URDU dataset.

---

Siddique Latif,
Jun 29, 2018 

---

**Original Dataset**: [Urdu-dataset]( https://github.com/siddiquelatif/urdu-dataset)

**DAGsHub Dataset:** [URDU emotions dataset by Siddique Latif ](https://dagshub.com/kingabzpro/URDU-Dataset)

**Photo** by [Allef Vinicius](https://unsplash.com/@seteph?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/pakistani?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

---

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*

