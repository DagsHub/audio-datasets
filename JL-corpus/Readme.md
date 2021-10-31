# JL-Corpus

![abc](https://images.unsplash.com/photo-1612232134966-a9b076b9fbe7?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2070&q=80)
credit: [Tengyart](https://unsplash.com/@tengyart)

The dataset is posted to [DagsHub](https://dagshub.com/hazalkl/JL-Corpus), where you may preview it before downloading it.

### About:
The aim of this work is to record an emotional speech database in New Zealand English, named as JL corpus.  This proposal explains the plan for the recording and the methods and database to be adopted for the process. This is further extended by the inclusion of the recording of the EGG signals as well, along with the speech signals. The aim of this work is to record an emotional speech database in New Zealand English, named as JL corpus. For further understanding the wide array of emotions embedded in human speech, they are introducing an emotional speech corpus. In contrast to the existing speech corpora, this corpus was constructed by maintaining an equal distribution of 4 long vowels in New Zealand English. This balance is to facilitate emotion related formant and glottal source feature comparison studies.  Also, the corpus has 5 secondary emotions along with 5 primary emotions. Secondary emotions are important in Human-Robot Interaction (HRI), where the aim is to model natural conversations among humans and robots. But there are very few existing speech resources to study these emotions,and this work adds a speech corpus containing some secondary emotions. 

### Structure:

The proposed database will have the voice from 4 speakers - 2 male and 2 female.

The sampling rate of the recording is set to be 44 kHz.

There will be 15 common sentences for different main emotions(15*5 sentences).

There will be 10 specific sentences for each sub-emotion(10*6 sentences).

These sentences will be recorded twice in two separate sessions, to generalize the possible time related mental variation and to ensure that the required emotion intensity level is consistent and that it is repeatable.

So, the total number of sentences for each person will be :

5 (main emotions) * 2 (repetitions) * 15 (sentences) + 6 (sub emotions) * 2 (repetitions) * 10 (sentences) = 150 + 120 = 270 sentences per person.

Total = 4 (number of speakers) * 270 = 1080 sentences.

The audio files are in `.wav` format

File naming rule:

(Gender)(speaker.ID)_(Emotion)_(Sentence.ID)(session.ID)

E.g:
+ `female1_angry_1a_1.wav`



### Authors:
Please use the corpus for emotional speech related studies. When you use it please include the citation as:

Jesin James, Li Tian, Catherine Watson, "An Open Source Emotional Speech Corpus for Human Robot Interaction Applications", in Proc. Interspeech, 2018.

---
You may get the dataset by clicking on the [link](https://www.kaggle.com/tli725/jl-corpus?select=README.md)