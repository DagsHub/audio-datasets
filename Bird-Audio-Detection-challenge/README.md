# Bird-Audio-Detection-challenge

![image](https://dagshub.com/kingabzpro/Bird-Audio-Detection-challenge/raw/master/asset/image.jpg)

**Detecting bird sounds in audio** is an important task for automatic wildlife monitoring, as well as in citizen science and audio library management. The current generation of software tools require manual work from the user: to choose the algorithm, to set the settings, and to post-process the results. This is holding bioacoustics back in embracing its “big data” era: let’s make this better!

In collaboration with the IEEE Signal Processing Society we propose a **research data challenge** for you to create a robust and scalable bird detection algorithm. We offer **new datasets** collected in real live bioacoustics monitoring projects, and an objective, standardised **evaluation framework** – and **prizes** for the strongest submissions.

**The subset of dataset (freefield1010) is uploaded to DagsHub: [Bird-Audio-Detection-challenge](https://dagshub.com/kingabzpro/Bird-Audio-Detection-challenge), enabling you to preview the dataset before downloading it.**

 

- **NEWS, July 2018: [read our paper covering the Bird Audio Challenge in full](https://doi.org/10.1111/2041-210X.13103)**
- NEWS, March 2018: a [new edition of the Bird Audio Detection challenge runs in 2018 as part of *DCASE 2018*](http://dcase.community/)

 

**Main links** for the original Bird Audio Detection challenge (2016/2017):

1. [View the results](http://machine-listening.eecs.qmul.ac.uk/bird-audio-detection-challenge-results/) online
2. [Download the data](http://machine-listening.eecs.qmul.ac.uk/bird-audio-detection-challenge/#downloads)
3. Read the academic papers:
   - A [full paper covering all the outcomes from the challenge](https://doi.org/10.1111/2041-210X.13103) (published in *Methods in Ecology and Evolution*, 2018)
   - Conference papers by challenge participants, presented at EUSIPCO 2017:
     - [Cakir et al](http://ieeexplore.ieee.org/document/8081508/) (joint winner of judges’ award)
     - [Thakur et al](http://ieeexplore.ieee.org/document/8081510/) (joint winner of judges’ award)
     - [Kong et al](http://ieeexplore.ieee.org/document/8081509/)
     - [Pellegrini](http://ieeexplore.ieee.org/document/8081506/)
     - [Adavanne et al](http://ieeexplore.ieee.org/document/8081505/)
     - [Grill and S](http://ieeexplore.ieee.org/document/8081512/)[chlüter](http://ieeexplore.ieee.org/search/searchresult.jsp?searchWithin="Authors":.QT.Jan Schlüter.QT.&newsearch=true) (strongest-performing system)
     - [Abrol et al](http://ieeexplore.ieee.org/document/8081510/)
   - [Conference survey paper](http://arxiv.org/abs/1608.03417) (MLSP 2016) – the paper in which we originally launched the challenge

There was also a [discussion](https://groups.google.com/forum/#!forum/bird-detection) forum used during the challenge.

## Task description and datasets

The task is to design a system that, given a short audio recording, returns a binary decision for the presence/absence of bird sound (bird sound of any kind). The output can be just “0” or “1”, but we encourage weighted/probability outputs in the continuous range [0,1] for the purposes of evaluation. For the main assessment we will use the well-known “Area Under the ROC Curve” ([AUC](https://en.wikipedia.org/wiki/Receiver_operating_characteristic#Area_under_curve)) measure for classification performance.

**Dataset 1: Field recordings (freefield1010) ** **[Dataset is available at DAGsHub]**

Our first dataset comes from [freefield1010](https://arxiv.org/abs/1309.5275) – a collection of over 7,000 excerpts from field recordings around the world, gathered by the [FreeSound](http://freesound.org/) project, and then standardised for research. This collection is very diverse in location and environment, and for the BAD Challenge we have newly annotated it for the presence/absence of birds.

**Dataset 2: Crowdsourced dataset (Warblr)**

Our second dataset comes from a UK bird-sound crowdsourcing research spinout called [Warblr](http://warblr.net/). From this initiative we have 10,000 ten-second smartphone audio recordings from around the UK. The audio totals around 44 hours duration. The audio will be published by Warblr under a Creative Commons licence. The audio covers a wide distribution of UK locations and environments, and includes weather noise, traffic noise, human speech and even human bird imitations. It is directly representative of the data that is collected from a mobile crowdsourcing initiative.

**Dataset 3: Remote monitoring dataset (Chernobyl)**

Our third dataset comes from the Natural Environment Research Council (NERC)-funded [TREE (Transfer-Exposure-Effects) research project](https://wiki.ceh.ac.uk/display/NRT/NERC+RATE+TREE+Home), which is deploying unattended remote monitoring equipment in the Chernobyl Exclusion Zone (CEZ). This academic investigation into the long-term effects of the Chernobyl accident on local ecology is led by Dr Wood. The project has captured approximately 10,000 hours of audio to date (since June 2015). The audio covers a range of birds and includes weather, large mammal and insect noise sampled across various CEZ environments, including abandoned village, grassland and forest areas.

The [task specification](http://machine-listening.eecs.qmul.ac.uk/bird-audio-detection-challenge-task-specification/) gives technical details of how participants will submit their analyses.

***Please note:*** we wish to encourage the development of generalisable and “tuning-free” methods by ensuring that testing data is recorded under ***different conditions*** than the publicly-available data. This helps ensure that the challenge addresses the needs identified in recent research for methods that can operate in unseen conditions. The training data will come from freefield1010 and Warblr, and the testing data from a mixture of data, predominantly from the Chernobyl dataset.

## Data downloads

Download the **development** data:

- freefield1010: • [[data labels](https://ndownloader.figshare.com/files/6035814)] • [[audio files](https://archive.org/download/ff1010bird/ff1010bird_wav.zip) (5.8 Gb zip)] (or [[via bittorrent](https://archive.org/download/ff1010bird/ff1010bird_archive.torrent)])
- Warblr: • [[data labels](https://ndownloader.figshare.com/files/6035817)] • [[audio files](https://archive.org/download/warblrb10k_public/warblrb10k_public_wav.zip) (4.3 Gb zip)] (or [[via bittorrent](https://archive.org/download/warblrb10k_public/warblrb10k_public_archive.torrent)])

and the **testing** data:

- Test set, from Chernobyl and Warblr: • [[audio files](https://archive.org/download/birdaudiodetectionchallenge_test/badchallenge_testdata_wavs.zip) (6.1 Gb zip)] (or [[via bittorrent](https://archive.org/download/birdaudiodetectionchallenge_test/birdaudiodetectionchallenge_test_archive.torrent)])
  – along with a blank submission file [csv](https://archive.org/download/birdaudiodetectionchallenge_test/badch_testset_blankresults.csv)

*(Thanks to [Figshare](https://figshare.com/) and [archive.org](https://archive.org/) for hosting data downloads.)*

## Directory

The dataset is small (6.33 GB) and simple to navigate as it has only single folder audio files. The `ff1010bird_labels.csv` file contains label [0,1] against audio files.  There are 7690 excerpts from field recordings around the world, gathered by the [FreeSound](http://freesound.org/) project, and then standardised for research. This collection is very diverse in location and environment, and for the BAD Challenge we have newly annotated it for the presence/absence of birds.

**Note**: *We have only uploaded freefield1010 to DVC server, to download entire dataset check the links in above sections.* 

```
<root directory>
    |
    .- README.md
    |
    .- LICENSE.txt
    |
    .- ff1010bird_labels.csv
    |
    .- Data/
          |
          .- 55.wav
          |
          .- 87.wav
          |
          .- 99.wav
          |
          ...
```

## How the challenge will work

The interface for submitting [results files](http://machine-listening.eecs.qmul.ac.uk/bird-audio-detection-challenge-task-specification/) will be a Kaggle-like interface designed for academic users. The main criterion for evaluating submissions will be the AUC, but we also aim to encourage computationally-efficient methods by recording the computation time taken.

As well as the public online challenge, we are also organising:

- A conference special session on the topic, with contributions from international experts.
- A journal special issue on the topic.

**Prizes:** There will be one prize of **£500** and one prize of **€500**, to be awarded to the strongest submissions. One prize will go to the submission with the best overall performance on the testing data (NB: to be eligible we will also require the teams to provide documentation / source code for their method – since, after all, the aim is to advance the state of the art). One prize will be the judges’ award, which will go to the submission which the judges feel has made a notable contribution to the topic. The organisers reserve the right to make the final decision on prize allocations, but please [ask](https://groups.google.com/forum/#!forum/bird-detection) if you have any queries.

## RESULTS

In revalidating the testing set, we examined those items with the strongest mismatch between manual and automatic detection, to determine which was in error: 500 presumed negative and 1,243 presumed positive items. This showed inter-rater disagreement in 16.6% of such cases predominantly, the most ambiguous cases with barely audible bird sounds with amplitude close to the noise threshold. Note that this percentage is not representative of disagreement across the whole dataset, but only on the “controversial” cases. We also observed that a strong mismatch according to the automatic detectors did not necessarily imply human mislabelling: some perceptually obvious data items could be consistently misjudged by algorithms. We will discuss algorithm errors further below. Through revalidation, the inter-rater reliability, measured via the AUC, was measured as 96.7%. This value provides an approximate upper limit for machine performance since it reflects the extent of ambiguity in the data according to human listeners’ perception.

The two baseline classifiers gave relatively good performance on the development data, the strongest at over 85% AUC in matched conditions, but generalised poorly. The simpler GMM-based baseline classifier showed consistently lower results than the more advanced classifier, as expected. It also showed strong resistance to overfitting in the sense that its performance on its training set was a very good predictor of its performance on a matched-conditions testing set. However, this was not sufficient to allow it to generalise to mismatched conditions, in which its performance degraded dramatically (Figure [1](https://besjournals.onlinelibrary.wiley.com/doi/10.1111/2041-210X.13103#mee313103-fig-0001)). The more advanced baseline classifier also degraded when tested in mismatched conditions, though to a lesser extent, attaining 74.8% AUC in the main evaluation.

[![image](https://besjournals.onlinelibrary.wiley.com/cms/asset/d4e8640d-7593-4f76-b6b1-687d62f64274/mee313103-fig-0001-m.png)](https://besjournals.onlinelibrary.wiley.com/cms/asset/96aeb10c-89a6-486e-9ac7-23fd721f8688/mee313103-fig-0001-m.jpg)

**Figure 1**

[Open in figure viewer](https://besjournals.onlinelibrary.wiley.com/doi/10.1111/2041-210X.13103#)[PowerPoint](https://besjournals.onlinelibrary.wiley.com/action/downloadFigures?id=mee313103-fig-0001&doi=10.1111%2F2041-210X.13103)

Final scores attained by the highest performing submission for each team. Error bars are estimated by bootstrap sampling. “skfl” and “smacpy” shown near the start are the baseline systems

## ACKNOWLEDGEMENTS

We thank Nick Beresford and Sergey Gashchak for their help with capturing the Chernobyl soundscape recordings, Paul Kendrick for preparation and annotation of Chernobyl data, Luciana Barçada for annotation of Chernobyl data, and Julien Ricard for programming and administering the challenge submission website. We also thank the many challenge participants for their enthusiastic effort. The Chernobyl data collection was undertaken within the TREE project ([www.ceh.ac.uk/TREE](http://www.ceh.ac.uk/TREE)), which is funded by the Natural Environment Research Council, the Environment Agency and Radioactive Waste Management Ltd.

## AUTHORS’ CONTRIBUTIONS

D.S., M.D.W., Y.S., and H.G. designed the data challenge study and its analysis; D.S., M.D.W., and H.P. provided datasets; H.G. led the creation of the challenge submission website; D.S. and H.P. performed tests of machine learning systems; D.S., H.G., and H.P. analysed the results; D.S. led the writing of the manuscript, with some sections by H.P. All authors contributed critically to the drafts and gave final approval for publication.

## DATA ACCESSIBILITY

- Development datasets: both audio and annotations are available under CC-BY-4.0 licences.warblrb10kaudio: https://archive.org/details/warblrb10k_publicff1010bird audio: https://archive.org/details/ff1010birdAnnotations: https://doi.org/10.6084/m9.figshare.3851466.v1
- Testing data (Chernobyl/warblrb10k): audio public, but annotations held back for future challenges. Audio: https://archive.org/details/birdaudiodetectionchallenge_test
- PolandNFC data: held back, in preparation for future challenge.
- Source code for baseline classifiers:GMM “smacpy” classifier (MIT licence): https://doi.org/10.5281/zenodo.1434195.skfl feature-learning (MIT licence): https://doi.org/10.7717/peerj.488/supp-1.
- Source code for the online submission website (MIT licence): https://doi.org/10.5281/zenodo.1434268
- Source code and papers for various of the systems submitted by challenge teams are available via http://c4dm.eecs.qmul.ac.uk/events/badchallenge_results (various licences). The strongest submission “bulbul” is available at https://doi.org/10.5281/zenodo.1434624 and described further in Grill and Schlüter ([2017](https://besjournals.onlinelibrary.wiley.com/doi/10.1111/2041-210X.13103#mee313103-bib-0015)).

## Organisers

- **Dr Dan Stowell,** Queen Mary University of London, London, UK.
- **Pr. Hervé Glotin,** Scaled Acoustic BioDiversity Dept, Univ. of Toulon & Inst. Univ. de France.
- **Pr. Yannis Stylianou,** Computer Science Dept, University of Crete.
- **Dr Mike Wood,** University of Salford, Greater Manchester, UK.

![Queen_Mary,_University_of_London_logo](http://machine-listening.eecs.qmul.ac.uk/wp-content/uploads/sites/26/2016/04/Queen_Mary_University_of_London_logo-1024x273.png) ![Univ Toulon Logo](http://www.univ-tln.fr/squelettes/images/logos/logo-utln.png) ![Univ Crete Logo](https://upload.wikimedia.org/wikipedia/en/f/f0/University_of_crete_logo.png) ![Univ Salford Logo](http://www.salford.ac.uk/__data/assets/image/0017/250064/logo-70.png)![Madics logo](http://machine-listening.eecs.qmul.ac.uk/wp-content/uploads/sites/26/2016/05/Logo-Madics-V5-300x99.jpg)

---

**Original Dataset**:  [[data labels](https://ndownloader.figshare.com/files/6035814)] • [[audio files](https://archive.org/download/ff1010bird/ff1010bird_wav.zip) ]

**DAGsHub Dataset:** [kingabzpro/Bird-Audio-Detection-challenge](https://dagshub.com/kingabzpro/Bird-Audio-Detection-challenge)

**Photo** by <a href="https://unsplash.com/@zmachacek?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Zdeněk Macháček</a> on <a href="https://unsplash.com/s/photos/bird?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

---

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*

