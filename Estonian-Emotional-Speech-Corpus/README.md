# Estonian-Emotional-Speech-Corpus
[![img](https://img.shields.io/badge/DOI-10.15155/3--00--0000--0000--0000--0001AL-red.svg)](https://doi.org/10.15155/3-00-0000-0000-0000-0001AL)[![img](https://img.shields.io/badge/doi-10.15155/EKI.000A-orange.svg)](https://doi.org/10.15155/3-00-0000-0000-0000-0001AL)[![img](https://img.shields.io/badge/license-CC%20BY--NC-blue.svg)](https://dagshub.com/kingabzpro/Estonian-Emotional-Speech-Corpus/src/master/LICENSE)[![img](https://img.shields.io/badge/download-metashare-ff69b4.svg)](https://metashare.ut.ee/repository/browse/estonian-emotional-speech-corpus/4d42d7a8463411e2a6e4005056b40024a19021a316b54b7fb707757d43d1a889/)

![image](https://dagshub.com/kingabzpro/Estonian-Emotional-Speech-Corpus/raw/master/asset/image.jpeg)

## General Information 
The Estonian Emotional Speech Corps (EEKK) is a corps created at the Estonian Language Institute within the framework of the state program "Estonian Language Technological Support 2006-2010", which contains read sentences of anger, joy and sadness as well as neutral sentences.The corpus contains 1,234 Estonian sentences that express anger, joy and sadness, or are neutral. Female voice, 44.1 KHz, 16Bit, Mono; wav, textgrid: phonemes, words, sentences.

**The similar version of dataset is uploaded to DagsHub: [Estonian-Emotional-Speech-Corpus](https://dagshub.com/kingabzpro/Estonian-Emotional-Speech-Corpus), enabling you to preview the dataset before downloading it.**

The corpus is based on the view that emotions are sufficiently well recognized by voice in natural unplayed speech, and that unplayed speech is a prerequisite for natural speech synthesis, see Iida et al. 2003.

## Organization

The dataset is small (339 MB) and simple to navigate as it has only single folder containing meta files and audio files. The corpus contains 1,234 Estonian sentences that express anger, joy and sadness, or are neutral. The folder also contains `.TestGrid` files of every audio file, which contains meta data of audio transcriptions and emotions. 

```
<root directory>
    |
    .- README.md
    |
    .- Dataset/
          |
          .- 37.TextGrid
          |
          .- 37.wav
          |
          .- 39.TextGrid
          |
          .- 39.wav
          | 
          ...
```

## Purpose

- be a reliable database for researching emotions in speech and writing;
- be the acoustic basis of corpus-based emotional text-to-speech synthesis;
- enable queries for language technology applications.
- The reliability of the corpus is ensured by perceptual tests: each sentence in the corpus is provided with perceptual test data on emotion recognition.
- The corpus is fully expandable: with readers, sentences, emotions, etc.

For more information on the housing, see Altrov 2007, 2008; Altrov, Willow Tree 2008, 2010; Altrov, Willow Tree 2012.

Current capabilities of the average user, queries
You can search the corps for sentences that carry an emotion of anger, joy, or sadness, and neutral sentences (see Reports).

Sentences are displayed in the text and can be heard by clicking.

The percentage of emotion perception is displayed next to the sentence.

Percentage can be given from which sentences are searched.

Queries can be restricted to only those sentences where

the text does not affect the emotion perception of the sentence
the text affects the perception of emotion in the sentence
You can save the sound and text of sentences (wav, textgrid). Housing labeling instructions can be found here.

## Technical description of the system

The corpus is implemented as a web-based application using freeware: Linux, PostgreSQL, Python, Praat, NLTK. All data except audio files is stored in a PostgreSQL database. The web interface and all data processing are performed using the programming language Python and the web environment Pylons. The application can be installed on both Windows and Linux environments. The web interface is in Estonian, English, Finnish and Latvian and can be easily adapted to other languages. Housing data can also be downloaded to the EMU call processing system. The currently available databases are listed in a format suitable for EMU here, and tips for installing EMU can be found here.

## References 
**Altrov, Rene 2007**. Creation of an emotional speech corpus for Estonian text-to-speech synthesis. Evaluation of text material on the example of anger. Master's thesis. University of Tartu.

**Altrov, Rene; Pajupuu, Hille 2008**. The Estonian Emotional Speech Corpus: Release 1. In: Proc. of the Third Baltic Conference on Human Language Technologies, František Čermak, Rūta Marcinkevičienė, Erika Rimkutė, Jolanta Zabarskaitė (eds.), 9-15. Vytautas Magnus University; Lithuanian Language Institute, Vilnius.

**Altrov, Rene; Pajupuu, Hille 2010**. Estonian Emotional Speech Corpus: Culture and Age in Selecting Corpus Testers. In: Human Language Technologies - The Baltic Perspective - Proc. of the Fourth International Conference Baltic HLT 2010, Inguna Skadiņa, Andrejs Vasiljevs (eds.), 25-32. Amsterdam: IOS Press.

**Altrov, Rene; Pajupuu, Hille 2012**. Estonian Emotional Speech Corpus: Theoretical base and implementation. In: 4th International Workshop on Corpora for Research on Emotion Sentiment & Social Signals (ES3), Devillers, L., Schuller, B., Batliner, A., Rosso, P., Douglas-Cowie, E., Cowie, R. , Pelachaud, C. (eds.), 50-53. Istanbul.

**Boersma, Paul; Weenink, David 2009**. Praat: doing phonetics by computer (Version 5.1.01) [Computer program]. Retrieved February 26, 2009.

**Iida, Akemi; Campbell, Nick; Higuchi, Fumito; Yasumura, Michiaki 2003**. A corpus-based speech synthesis system with emotion. Speech Communication, 40, 161–187. 

## Attribution

If you use the Estonian Emotional Speech Corpus for your research, please cite the following paper: Altrov, Rene; Pajupuu, Hille 2012. Estonian Emotional Speech Corpus: Theoretical base and implementation. In: 4th International Workshop on Corpora for Research on Emotion Sentiment & Social Signals (ES3), Devillers, L., Schuller, B., Batliner, A., Rosso, P., Douglas-Cowie, E., Cowie, R., Pelachaud, C.(eds.),50-53. Istanbul.

## License 

It's licensed under the [Creative Commons BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).

## Licensors

[Eesti Keele Instituut, Institute of the Estonian Language ![img](https://metashare.ut.ee/site_media/css/sexybuttons/images/icons/silk/vcard.png)](https://metashare.ut.ee/repository/browse/estonian-emotional-speech-corpus/4d42d7a8463411e2a6e4005056b40024a19021a316b54b7fb707757d43d1a889/#)

http://portaal.eki.ee/

Eesti Keele Instituut, Institute of the Estonian Language

[eki@eki.ee](mailto:eki@eki.ee)

Roosikrantsi 6

10119 Tallinn

Estonia

Tel.: +372 6177 500

## Contact Person

[Hille Pajupuu ![img](https://metashare.ut.ee/site_media/css/sexybuttons/images/icons/silk/vcard.png)](https://metashare.ut.ee/repository/browse/estonian-emotional-speech-corpus/4d42d7a8463411e2a6e4005056b40024a19021a316b54b7fb707757d43d1a889/#)

Eesti Keele Instituut, Institute of the Estonian Language

[Hille.Pajupuu@eki.ee](mailto:Hille.Pajupuu@eki.ee)

http://portaal.eki.ee/

Roosikrantsi 6

10119 Tallinn

Estonia

[eki@eki.ee](mailto:eki@eki.ee)

Tel.: +372 6177 500

---

**Original Dataset**: [Estonian Emotional Speech Corpus](https://metashare.ut.ee/repository/download/4d42d7a8463411e2a6e4005056b40024a19021a316b54b7fb707757d43d1a889/)

**DAGsHub Dataset:**[kingabzpro/Estonian-Emotional-Speech-Corpus](https://dagshub.com/kingabzpro/Estonian-Emotional-Speech-Corpus)  

**Photo** by <a href="https://unsplash.com/@iliched?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Ilya Orehov</a> on <a href="https://unsplash.com/s/photos/estonian?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

---

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*
