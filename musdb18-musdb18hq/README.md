# MUSDB18 & MUSDB18HQ 
Multi-track music dataset for music source separation. There are 2 version of MUSDB18, the compressed and the uncompressed(HQ).

## [MUSDB18](https://dagshub.com/kinkusuma/musdb18/src/master/compressed) - a corpus for music separation

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1117372.svg)](https://zenodo.org/record/1117372#.YWfyeBx8rIV)

The sigsep musdb18 data set consists of a total of 150 full-track songs of different styles and includes both the stereo mixtures and the original sources, divided between a training subset and a test subset.

Its purpose is to serve as a reference database for the design and the evaluation of source separation algorithms. The objective of such signal processing methods is to estimate one or more sources from a set of mixtures, e.g. for karaoke applications. It has been used as the official dataset in the professionally-produced music recordings task for SiSEC 2018, which is the international campaign for the evaluation of source separation algorithms.

musdb18 contains two folders, a folder with a training set: “train”, composed of 100 songs, and a folder with a test set: “test”, composed of 50 songs. Supervised approaches should be trained on the training set and tested on both sets.

All files from the musdb18 dataset are encoded in the Native Instruments stems format (.mp4). It is a multitrack format composed of 5 stereo streams, each one encoded in AAC @256kbps. These signals correspond to:

* 0 - The mixture,
* 1 - The drums,
* 2 - The bass,
* 3 - The rest of the accompaniment,
* 4 - The vocals.

For each file, the mixture correspond to the sum of all the signals. All signals are stereophonic and encoded at 44.1kHz.

As the MUSDB18 is encoded as STEMS, it relies on ffmpeg to read the multi-stream files. We provide a python wrapper called stempeg that allows to easily parse the dataset and decode the stem tracks on-the-fly.

## [MUSDB18-HQ](https://dagshub.com/kinkusuma/musdb18/src/master/dataset) - an uncompressed version of MUSDB18

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3338373.svg)](https://zenodo.org/record/3338373#.YWfvIBx8rIU)

MUSDB18-HQ is the uncompressed version of the MUSDB18 dataset. It consists of a total of 150 full-track songs of different styles and includes both the stereo mixtures and the original sources, divided between a training subset and a test subset.

Its purpose is to serve as a reference database for the design and the evaluation of source separation algorithms. The objective of such signal processing methods is to estimate one or more sources from a set of mixtures, e.g. for karaoke applications. It has been used as the official dataset in the professionally-produced music recordings task for SiSEC 2018, which is the international campaign for the evaluation of source separation algorithms.

musdb18-hq contains two folders, a folder with a training set: “train”, composed of 100 songs, and a folder with a test set: “test”, composed of 50 songs. Supervised approaches should be trained on the training set and tested on both sets.

All files from the musdb18-hq dataset are saved as uncompressed wav files. Within each track folder, the user finds

* mixture.wav
* drums.wav
* bass.wav,
* other.wav,
* vocals.wav

All signals are stereophonic and encoded at 44.1kHz.

## LICENSE

MUSDBHQ: is provided for educational purposes only and the material contained in them should not be used for any commercial purpose without the express permission of the copyright holders:

* 100 tracks are taken from the DSD100 data set, which is itself derived from The ‘Mixing Secrets’ Free Multitrack Download Library. Please refer to this original resource for any question regarding your rights on your use of the DSD100 data.
* 46 tracks are taken from the MedleyDB licensed under Creative Commons (BY-NC-SA 4.0).
* 2 tracks were kindly provided by Native Instruments originally part of their stems pack.
* 2 tracks a from from the Canadian rock band The Easton Ellises as part of the heise stems remix competition, licensed under Creative Commons (BY-NC-SA 3.0).

## REFERENCE

If you use the MUSDB dataset for your research - Cite the MUSDB18 Dataset

```
@misc{MUSDB18HQ,
  author       = {Rafii, Zafar and
                  Liutkus, Antoine and
                  Fabian-Robert St{\"o}ter and
                  Mimilakis, Stylianos Ioannis and
                  Bittner, Rachel},
  title        = {{MUSDB18-HQ} - an uncompressed version of MUSDB18},
  month        = dec,
  year         = 2019,
  doi          = {10.5281/zenodo.3338373},
  url          = {https://doi.org/10.5281/zenodo.3338373}
}
```

If compare your results with SiSEC 2018 Participants - Cite the SiSEC 2018 LVA/ICA Paper

```
@inproceedings{SiSEC18,
  author="St{\"o}ter, Fabian-Robert and Liutkus, Antoine and Ito, Nobutaka",
  title="The 2018 Signal Separation Evaluation Campaign",
  booktitle="Latent Variable Analysis and Signal Separation:
  14th International Conference, LVA/ICA 2018, Surrey, UK",
  year="2018",
  pages="293--305"
}
```


### Check this dataset in:

* Original source:
  * [MUSDB18](https://zenodo.org/record/1117372#.YWfyeBx8rIV)
  * [MUSDB18HQ](https://zenodo.org/record/3338373#.YWfvIBx8rIU)

* DagsHub: [musdb18-dataset](https://dagshub.com/kinkusuma/musdb18-dataset)
