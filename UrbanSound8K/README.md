# UrbanSound8K-Labeled_Urban_Sound_Excerpts_Dataset

### Paper: [A Dataset and Taxonomy for Urban Sound Research](http://www.justinsalamon.com/uploads/4/3/9/4/4394963/salamon_urbansound_acmmm14.pdf)
### DagsHub Repository: [UrbanSound8K-Labeled_Urban_Sound_Excerpts_Dataset](https://dagshub.com/Rutam21/UrbanSound8K-Labeled_Urban_Sound_Excerpts_Dataset)

![DagsHub Hacktoberfest Cover](https://user-images.githubusercontent.com/66431403/192983164-b3d6d556-ac69-4fb8-8aef-726a4386406a.png)

## About

Urban Sound 8K is an audio dataset that contains 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, enginge_idling, gun_shot, jackhammer, siren, and street_music. The classes are drawn from the urban sound taxonomy. All excerpts are taken from field recordings uploaded to www.freesound.org.

## Dataset

8732 audio files of urban sounds (see description above) in WAV format. The sampling rate, bit depth, and number of channels are the same as those of the original file uploaded to Freesound (and hence may vary from file to file).

### META-DATA FILES INCLUDED

This file contains meta-data information about every audio file in the dataset. This includes:

* **slice_file_name:** 
The name of the audio file. The name takes the following format: [fsID]-[classID]-[occurrenceID]-[sliceID].wav, where:
    - [fsID] = the Freesound ID of the recording from which this excerpt (slice) is taken
    - [classID] = a numeric identifier of the sound class (see description of classID below for further details)
    - [occurrenceID] = a numeric identifier to distinguish different occurrences of the sound within the original recording
    - [sliceID] = a numeric identifier to distinguish different slices taken from the same occurrence

* **fsID:**
The Freesound ID of the recording from which this excerpt (slice) is taken

* **start:**
The start time of the slice in the original Freesound recording

* **end:**
The end time of slice in the original Freesound recording

* **salience:**
A (subjective) salience rating of the sound. 1 = foreground, 2 = background.

* **fold:**
The fold number (1-10) to which this file has been allocated.

* **classID:**
A numeric identifier of the sound class:
    - 0 = air_conditioner
    - 1 = car_horn
    - 2 = children_playing
    - 3 = dog_bark
    - 4 = drilling
    - 5 = engine_idling
    - 6 = gun_shot
    - 7 = jackhammer
    - 8 = siren
    - 9 = street_music

* **class:**
The class name: air_conditioner, car_horn, children_playing, dog_bark, drilling, engine_idling, gun_shot, jackhammer, 
siren, street_music.

## Acknowledgement

When UrbanSound or UrbanSound8K is used for academic research, we would highly appreciate it if scientific publications of works partly based on these datasets cite the aforementioned publication.

The creation of the datasets was supported by a seed grant by NYU's Center for Urban Science and Progress (CUSP).

## CONDITIONS OF USE

Datasets compiled by Justin Salamon, Christopher Jacoby and Juan Pablo Bello. All files come from www.freesound.org. 
Please see FREESOUNDCREDITS.txt (included in the dataset) for an attribution list.
 
The UrbanSound and UrbanSound8K datasets are offered free of charge for non-commercial use only under the terms of the Creative Commons Attribution Noncommercial License (by-nc), version 3.0: http://creativecommons.org/licenses/by-nc/3.0/
 
The datasets and their contents are made available on an "as is" basis and without warranties of any kind, including without limitation satisfactory quality and conformity, merchantability, fitness for a particular purpose, accuracy or completeness, or absence of errors. Subject to any liability that may not be excluded or limited by law, NYU is not liable for, and expressly excludes, all liability for loss or damage however and whenever caused to anyone by any use of the UrbanSound or UrbanSound8K datasets or any part of them.


## Citation

```
@inproceedings{Salamon:UrbanSound:ACMMM:14,
    Address = {Orlando, FL, USA},
    Author = {Salamon, J. and Jacoby, C. and Bello, J. P.},
    Booktitle = {22nd {ACM} International Conference on Multimedia (ACM-MM'14)},
    Month = {Nov.},
    Pages = {1041--1044},
    Title = {A Dataset and Taxonomy for Urban Sound Research},
    Year = {2014}}
```
