# FSDnoisy18k-Open_Audio_Dataset

### Paper: [Learning Sound Event Classifiers from Web Audio with Noisy Labels](https://arxiv.org/pdf/1901.01189v2.pdf)
### DagsHub Repository: [FSDnoisy18k-Open_Audio_Dataset](https://dagshub.com/Rutam21/FSDnoisy18k-Open_Audio_Dataset)

![DagsHub Hacktoberfest Cover](https://user-images.githubusercontent.com/66431403/192983164-b3d6d556-ac69-4fb8-8aef-726a4386406a.png)

## About

The FSDnoisy18k dataset is an open dataset containing 42.5 hours of audio across 20 sound event classes, including a small amount of manually-labeled data and a larger quantity of real-world noisy data. The audio content is taken from Freesound, and the dataset was curated using the Freesound Annotator. The noisy set of FSDnoisy18k consists of 15,813 audio clips (38.8h), and the test set consists of 947 audio clips (1.4h) with correct labels. The dataset features two main types of label noise: in-vocabulary (IV) and out-of-vocabulary (OOV). IV applies when, given an observed label that is incorrect or incomplete, the true or missing label is part of the target class set. Analogously, OOV means that the true or missing label is not covered by those 20 classes.

## Dataset

The 20 classes of FSDnoisy18k are drawn from the AudioSet Ontology and are selected based on data availability as well as on their suitability to allow the study of label noise. For example:

- Some classes are selected because the tags typically used to describe them can also be used for other audio material. Hence when the content for these classes is retrieved by the typical user-provided tags (as is our case), it is likely to feature a certain amount of label noise. Some examples of these classes are: Bass guitar, Crash Cymbal, Engine, Fire, etc.

- Some classes are chosen because their clips are typically outdoor field-recordings, where several sound sources are expected to be present (although it is likely that only the most predominant(s) are indeed tagged); for example: Rain, Fireworks, Slam, Fire, etc.

- Some pairs of classes are chosen due to their relation. For example, Slam and Squeak are often the outcome of one physical phenomenon (cloosing a door), hence they may co-occur in a clip despite sometimes only one may be tagged. Another example is Wind and Rain.

They are listed in the following Table, along with the number of audio clips per class.

|Class|train-clean|train-noisy|test|
|-|-|-|-|			
|Acoustic guitar|102 / 11|896 / 124|42 / 4|
|Bass guitar|106 / 11|1000 / 142|71 / 5|
|Clapping|82 / 3|846 / 104|57 / 4|
|Coin (dropping)|170 / 7|589 / 57|70 / 4|
|Crash cymbal|76 / 6|1000 / 105|52 / 4|
|Dishes, pots, and pans|83 / 4|764 / 105|56 / 3|
|Engine|137 / 20|995 / 172|49 / 10|
|Fart|71 / 2|687 / 43|30 / 1|
|Fire|81 / 7|751 / 132|54 / 5|
|Fireworks|51 / 4|331 / 55|30 / 3|
|Glass|157 / 12|998 / 123|54 / 3|
|Hi-hat|81 / 3|911 / 45|38 / 1|
|Piano|96 / 12|1000 / 174|72 / 8|
|Rain|65 / 9|443 / 117|36 / 6|
|Slam|78 / 3|1000 / 129|53 / 2|
|Squeak|67 / 4|931 / 116|31 / 2|
|Tearing|62 / 4|428 / 54|30 / 3|
|Walk, footsteps|77 / 7|1000 / 206|52 / 6|
|Wind|64 / 7|993 / 276|40 / 5|
|Writing|66 / 8|250 / 48|30 / 4|

## Citation

```
Eduardo Fonseca, Manoj Plakal, Daniel P. W. Ellis, Frederic Font, Xavier Favory, and Xavier Serra, “Learning Sound Event Classifiers from Web Audio with Noisy Labels”, arXiv preprint arXiv:1901.01189, 2019
----
Eduardo Fonseca, Jordi Pons, Xavier Favory, Frederic Font, Dmitry Bogdanov, Andres Ferraro, Sergio Oramas, Alastair Porter, and Xavier Serra, “Freesound Datasets: A Platform for the Creation of Open Audio Datasets”, In Proceedings of the 18th International Society for Music Information Retrieval Conference, Suzhou, China, 2017
----
```

