# BAVED Dataset

Basic Arabic Vocal Emotions Dataset (BAVED) is a datasetthat contains an arabic words spelled in diffrent levels of emotions recorded in an audio/wav format.

## About the dataset

This data set contains a 7 arabic words identified and named as the following:

0- اعجبني

1- لم يعجبني

2- هذا

3- الفيلم

4- رائع

5- مقول

6- سيئ

Each of the previous words is recorded in three levels of emotions. Level 0 is when the speaker is expressing a low level of emotion, this is similar to feeling tired or feeling down. Level 1 is the the standered level, it is the way the speaker speaks daily where he/she is expressing a neutral emotions,finally the level 2 emotion, its when the speaker is expressing a high level of positive or negative emotions (happiness, joy, sadness, anger, etc…).

    Number of records: 1935
    NUmber of speakers: 61
    NUmber of male speakers: 45
    NUmber of female speakers: 16
    Data-set size: 97.8 MB

## Files meta-data

Note: the samples were recorded in diffrent stats, then they were normalized and formated into the following parameters:

    type: audio/wav (original: video/mp4 or audio/wav)
    Sample rate: 16 kHz (original: 48 kHz or higher frequencies)
    Number of channels: 1 (original: 2 channels)
    Bitrate: 256 kbit/s (original: 512 kbit/s)

## Naming

the samples in this dataset are named as the following:

speakerid(int) - speakergender(m or f) - speakerage(int) - spokenword(int between 0 and 6) - spokenemotion(int between 0 and 2) - recordid(int)

## Usage instructions

This dataset is mainly for a basic arabic speech recognition, and arabic vocal emotions detection,it shall give good results if trainned and tested for one of the previous purposes. Keep in mind that this dataset in its first version is limited to 7 wordes and three levels of emotions, so a commercial use won't probably be a good idea.

Even though this data-set includes the information about the age and gender of each speaker it is not very recommanded to build a model upon that, since the number of male speakers is almost 3 times more than the number of female speakers,and since the ages of the speakers are between 18 and 23 with some exceptions.


**Source of the database [Basic Arabic Vocal Emotions Dataset](https://www.kaggle.com/a13x10/basic-arabic-vocal-emotions-dataset)**  
**Check this database in [Dagshub](https://dagshub.com/kinkusuma/basic-arabic-vocal-emotions-dataset)**
