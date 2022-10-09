# LEGO-Spoken-Dialogue-Corpus

## 1) General information

The LEGOv2 database is a parameterized and annotated version of the CMU Let’s Go database from 2006 and 2007.

This spoken dialogue corpus contains interactions captured from the CMU Let’s Go (LG) System by Carnegie Mellon University in 2006 and 2007. It is based on raw log-files from the LG system.

The corpus has been parameterized and annotated by the Dialogue Systems Group at Ulm University, Germany.

#### This version has sections uploaded to DagsHub, enabling you to preview the dataset before downloading it.

## 2) Structure

The corpus comes with both, MySQL-database dumps and CSV files.

The mysql-dump can be imported right away in any MySQL database.
CSV files can be imported e.g. in Excel, Matlab, R, Weka, SPSS and other SQL databases than mysql.

- `interactions.csv/interactions-Table`: each line contains a system-user exchange, parameterized with 53 interaction parameters

- Use callid to join with call-Table

Furthermore, the file contains *`EmotionalState`* annotations and *`Interaction Quality`* annotations, see below. For interaction quality please refer 
to [Schmitt et al., 2011]

- `calls.csv/calls-Table`: each line contains information affecting the entire call. Primary key: callid

The file contains *`gender`*, *`age`* and *`dialogue outcome`* annotations that can be used as target variable to predict task completion.

- `acoustics.csv/acoustics-Table`: each line contains basic acoustic and prosodic features extracted on the full utterance. Extraction has been 
done with the Praat software; see [Schmitt2009] for details.


The LEGO Spoken Dialogue Corpus has the following directory structure:

### Files organization

```
license.txt -> license file
readme.txt -> this file
interaction_parameters.pdf -> Description of interaction parameters 
|
|---- audio -> wav files with user utterances and full recordings
|
|---- corpus
		|
		|---- csv   -> CSV-files with interactions.csv, acoustics.csv and calls.csv
		|---- mysql -> mysql dump
 ```

## 3) More information

- Number of Calls: 548
- Number of System-User Exchanges: 13,836


Interaction Quality [Schmitt2011]:

- Number of Calls with IQ Annotations from all Raters: 	401
- Number of Exchanges with IQ Annotations from all Raters: 9,638

Annotation Scheme: 
- 1: extremely unsatisfied
- 2: strongly unsatisfied
- 3: unsatisfied 
- 4: slightly unsatisfied
- 5: satisfied

------------------------------------------------------------------------------------------------------------------------
#### Rater guidelines for annotating Interaction Quality

1. The rater should try to mirror the users point of view on the interaction as objectively as possible.
2. An exchange consists of the system prompt and the user response. Due to system design, the latter is not always present.
3. The IQ score is defined on a 5-point scale with “1=bad”, “2=poor”, “3=fair”, “4=good” and “5=excellent”.
4. The Interaction Quality is to be rated for each exchange in the dialogue. The dialogue’s specific history should be minded.
For Example, a dialogue that has proceeded fairly poor for a long time, should require some time to recover.
5. A dialogue always starts with an Interaction Quality score 5.
6. The first user input should also be rated with 5, since until this moment, no rateable interaction has taken place.
7. A request for help does not invariably cause a lower Interaction Quality, but can result in it.
8. In general, the score from one exchange to the following exchange is increased or decreased by one point at the most.
9. Exceptions, where the score can be decreased by two points, are e.g. hot anger or sudden frustration. The rater’s
perception is decisive here.
10. Also, if the dialogue obviously collapses due to system or user behavior, the score can be set to 1 immediately. An
example is a reasonable frustrated sudden hang-up.
11. Anger does not need to influence the score, but can. You should try to figure out whether it might be caused by the
dialogue behavior or not.
12. In the case a user realizes that he should adapt his dialogue strategy to obtain the desired result or information and
succeeded that way, the Interaction Quality score can be raised up to two points per turn. In a manner of speaking, he
realizes that he caused the poor Interaction Quality by himself.
13. If the system does not reply with a bus schedule to a specific user query and prompts that the request is out of scope, this
can be considered as completed task and therefore does not need to affect the Interaction Quality.
14. If a dialogue consists of several independent queries, each query’s quality is to be rated independently. The dialogues
history shouldnt be minded when a new query begins. But the score provided for the first exchange should be equal to
the last label of the previous query.
15. If a dialogue proceeds fairly poor for a long time, the rater should consider to increase the score more slowly if its getting
better. Also, in general, he or she should observe the remaining dialogue more critical.
16. If a constantly low-quality dialogue finishes with a reasonable result, the Interaction Quality should be increased.

------------------------------------------------------------------------------------------------------------------------
#### Emotional States:

- Number of Calls with Emotion Annotations: 				302
- Number of Raters for Emotion Annotation: 				1

Annotation Scheme: friendly, neutral, slightly angry, angry, very angry


## 4) Acknowledgements

To cite the corpus, please use the following two publications:

```
[Schmitt2012] 
A. Schmitt, S. Ultes and W. Minker
A Parameterized and Annotated Spoken Dialog Corpus of the CMU Let's Go Bus Information System
International Conference on Language Resources and Evaluation (LREC), Istanbul, Turkey, pp. 3369--3373, May 2012
```

```
[Ultes2015] 
S. Ultes, A. Schmitt, M. J. Platero Sánchez and W. Minker
Analysis of an Extended Interaction Quality Corpus
International Workshop On Spoken Dialogue Systems (IWSDS), Busan, Korea, January 2015
submitted
```

References:

```
[Esenazi2008] Maxine Eskenazi, Alan W Black, Antoine Raux, and Brian Langner
Let’s Go Lab: a platform for evaluation of spoken dialog systems with real world users
in: Proceedings of Interspeech 2008 Conference, Brisbane, Australia`
```

```
[Schmitt2011] Alexander Schmitt, Benjamin Schatz and Wolfgang Minker, 
MODELING AND PREDICTING QUALITY IN SPOKEN HUMAN-COMPUTER INTERACTION, 
in: Proceedings of the SIGDIAL 2011 Conference, 
Association for Computational Linguistics, 2011`
```

```
[Schmitt2009]
A. Schmitt, T. Heinroth and J. Liscombe
On NoMatchs, NoInputs and BargeIns: Do Non-Acoustic Features Support Anger Detection?
Proceedings of the SIGDIAL 2009 Conference, Association for Computational Linguistics, London, UK, pp. 128--131, 2009
```


------------------------------------------------------------------------------------------------------------------------


### [DagsHub Dataset](https://dagshub.com/arnavr.neo/LEGO-Spoken-Dialogue-Corpus)

### *This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/dagshub-x-hacktoberfest-2022/)*.
