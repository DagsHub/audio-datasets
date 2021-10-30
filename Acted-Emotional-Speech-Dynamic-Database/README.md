# Acted-Emotional-Speech-Dynamic-Database

Acted Emotional Speech Dynamic Database is a Speech Emotion Recognition Dataset publically available for research purposes.

![cover](https://i0.wp.com/m3c.web.auth.gr/wp-content/uploads/2020/11/Asset-3pale.png?w=435)

## Speech Emotion Recognition

Speech Emotion Recognition (SER) is the process of extracting emotional paralinguistic information from speech. It is a field with growing interest and potential applications in Human-Computer Interaction, content management, social interaction, and as an add-on module in Speech Recognition and Speech-To-Text systems. The performance of such applications depends a lot on a high-quality speech emotion recognition dataset.

Text-independent automated SER relies on the specific attributes of speech audio signals. In such an elusive task as SER, typically a data-driven approach is followed. This means that models are trained on data. As a consequence, the performance of SER models is inextricably linked to the quality and the organization of the provided dataset.

**The similar version of dataset is uploaded to DagsHub: [Acted-Emotional-Speech-Dynamic-Database](https://dagshub.com/kingabzpro/Acted-Emotional-Speech-Dynamic-Database), enabling you to preview the dataset before downloading it.**

## A Public Speech Emotion Recognition Dataset

Databases of emotional speech are divided into two main categories, the ones that contain utterances of acted emotional speech and the ones that contain spontaneous emotional speech. Both categories have benefits and limitations.

The Acted Emotional Speech Dynamic Database (**AESDD**) is a publically available speech emotion recognition dataset. It contains utterances of acted emotional speech in the *Greek* language.

The motive for the creation of the database was the absence of a publically available high-quality database for SER in Greek, a realization made during the research on an emotion-triggered lighting framework for theatrical performance [1]. The database utterances with five emotions: ***anger***, ***disgust***, ***fear***, ***happiness,*** and ***sadness***.

The first version of the speech emotion recognition dataset was created in collaboration with a group of professional actors, who showed vivid interest in the proposed framework. Dynamic (in AESDD) refers to the intention of constantly expanding the database through the contribution of actors and performers that are involved, or interested in the project. While the call for contribution addresses to actors, the SER models that are trained on the AESDD are not exclusively performance-oriented.

The first version of the AESDD was presented in [2].

In [4], subjective evaluation experiments were carried out on the database, to assess human accuracy in recognizing the intended emotion in AESDD utterances. The accuracy of human listeners was estimated at around **74%**.

## Organisation 

There are five folders, named after the five emotion classes.
Every file name in the databased is in the following form:

- xAA (B) where x is the first letter of the emotion (a--> anger, h--> happiness etc.)
- AA is the number of the utterance (01,02...20)
- B is the number of the speaker (1 --> 1st speaker, 2 --> 2nd speaker etc)
- e.g. 'a03 (4).wav' is the 3rd utterance spoken by the 4th speaker with anger

In the case where two takes were qualified for the same utterance, they are distinguished with a lower case letter.

e.g. 'f18 (5).wav' and 'f18 (5)b.wav' are two different versions of the 5th actor saying the 18th utterance with fear.

## Results

 The conducted machine learning experiments were dependent on the classification scheme of the five emotional states of the  labeled instances, which represent the five output classes of the speech emotion recognition problem. Several classifiers were tested while using the WEKA environment, as well as the Matlab’s Classification Learner Toolbox.  The classification models were trained and validated by the input feature values. The tested algorithms included Multi-Class  Logistic Regression (Log.Reg.), Multi-Layer Perceptrons (MLP), Support Vector Machines (SVM) with polynomial kernel,  Logistic Model Trees (LMT) and a Subspace Ensemble Learning classifier (Ensemble) with 30 Discriminant Learners. The 10-fold  cross-validation technique was employed for training the algorithmic models, as well as to compute the respective performances by  the extracted confusion matrices (in terms of the ratios of the correctly classified instances to the total number of input samples or  the respective class size). The classification accuracy results (P) are depicted in Fig.1 for the five emotion classes (anger, disgust,  fear, happiness, sadness) along with the overall performance of the implemented training algorithm

![image-20211019174543577](https://dagshub.com/kingabzpro/Acted-Emotional-Speech-Dynamic-Database/raw/master/asset/image1.png)

**Fig. 1 Classification results for the personalized database for different classifiers and classes**

![image-20211019174355659](https://dagshub.com/kingabzpro/Acted-Emotional-Speech-Dynamic-Database/raw/master/asset/image2.png)

**Fig. 2 Compared results between the personalized emotional speech dataset and the augmented AESDD generalized dataset**

While observing Figure 1, the Ensemble Learning classifier scored the highest performance rates for the given dataset.  Thereafter, the personalized database that was created for the current work was integrated into the AESDD database, serving in  the same time the augmentation process. As mentioned before, the AESDD contains around 500 utterances from 5 different  actors, consequently the addition resulted in the a total number of 600 recorded phrases of emotional speech. The same  experimental procedure of classification and evaluation was followed for the augmented generalized dataset, and the  classification accuracy results are presented in Fig.2, in contradiction to the personalized dataset results.

## Acknowledgements

Part of this research has been financially supported by General Secretariat for Research and Technology (GSRT) and the  Hellenic Foundation for Research and Innovation (HFRI), which supports N. Vryzas’ PhD research. (Scholarship Code: 1900).

## Publications

1. Vryzas, N., Liatsou, A., Kotsakis, R., Dimoulas, C., & Kalliris, G. (2017, August). Augmenting Drama: A Speech Emotion-Controlled Stage Lighting Framework. In *Proceedings of the 12th International Audio Mostly Conference on Augmented and Participatory Sound and Music Experiences* (p. 8). ACM.
2. Vryzas, N., Kotsakis, R., Liatsou, A., Dimoulas, C. A., & Kalliris, G. (2018). Speech emotion recognition for performance interaction. *Journal of the Audio Engineering Society*, *66*(6), 457-467.
3. Vryzas, N., Vrysis, L., Kotsakis, R., & Dimoulas, C. (2018, September). Speech emotion recognition adapted to multimodal semantic repositories. In *2018 13th International Workshop on Semantic and Social Media Adaptation and Personalization (SMAP)* (pp. 31-35). IEEE.
4. Vryzas, N., Matsiola, M., Kotsakis, R., Dimoulas, C., & Kalliris, G. (2018, September). Subjective Evaluation of a Speech Emotion Recognition Interaction Framework. In *Proceedings of the Audio Mostly 2018 on Sound in Immersion and Emotion* (p. 34). ACM.

## Download

The last version of the AESDD, as well as tools and documentation on the way the database is organized, can be found in the following link:

[Acted Emotional Speech Dynamic Database](https://mega.nz/#F!0ShVXY7C!-73kVoK05OjTPEA95UUvMw)

If you use the AESDD for scientific research please cite **[2]** and **[4]**.

## Contribute to the AESDD Speech Emotion Recognition Datasets

The SpeechEmotionRecognition.xyz project aims at the formation of an open-sourced, anonymized multilingual speech emotion recognition datasets. The recordings of emotional speech that are submitted to the site, will be validated, and be provided publically for research non-commercial purposes.

The resulting dataset will be an extension of the Acted Emotional Speech Dynamic Database (AESDD).

Volunteers can contribute by recording their voice online at

[https://speechemotionrecognition.xyz](https://speechemotionrecognition.xyz/)

fb: https://www.facebook.com/Speech-Emotion-Recognition-109562454044394/?modal=admin_todo_tour

---

**Original Dataset:** [Acted Emotional Speech Dynamic Database](https://mega.nz/#F!0ShVXY7C!-73kVoK05OjTPEA95UUvMw)

**DAGsHub Dataset:** [kingabzpro/Acted-Emotional-Speech-Dynamic-Database](https://dagshub.com/kingabzpro/Acted-Emotional-Speech-Dynamic-Database)

---

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*