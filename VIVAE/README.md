
# The Variably Intense Vocalizations of Affect and Emotion Corpus (VIVAE)


![image](../assets/VIVAE/Photo.jpg)

**Image credit:** [Tengyart](https://unsplash.com/@tengyart) on [Unsplash](https://unsplash.com/)

**The dataset is uploaded to DagsHub: [VIVAE](https://dagshub.com/mert.bozkirr/VIVAE), enabling you to preview the dataset before downloading it.**

## Summary
The Variably Intense Vocalizations of Affect and Emotion Corpus (VIVAE) consists of a set of human non-speech emotion vocalizations. The full set, comprising 1085 audio files, features eleven speakers expressing three positive (achievement/ triumph, sexual pleasure, and surprise) and three negative (anger, fear, physical pain) affective states, each parametrically varied from low to peak emotion intensity. The smaller core set of 480 files represents a fully crossed subsample of the full set (6 emotions x 4 intensities x 10 speakers x 2 items) selected based on judged authenticity. 

</br>

## Construction and validation

Recordings took place at the Berklee College of Music in Boston MA, USA. The VIVAE full set contains 1085 files (i.e., all recordings that passed an acoustic quality check and were free of linguistic content). The core set was selected based on authenticity judgements collected throughout the technical validation of the dataset. The technical validation comprises data from 30 individuals providing emotion, intensity, and authenticity judgements. Details on the construction and perceptual evaluation will be shared in an academic paper. Please contact the authors for any questions at natalie.holz@ae.mpg.de.



## File summary

The recordings are digitized at a 44.1-kHz sampling rate and 16-bit resolution.

Each of the 1085 VIVAE files has a unique filename following the file naming convention: [Speaker_Emotion_Intensity_Item-ID.wav]. The filename consists of a 4-part identifier (e.g., S04_surprise_peak_10.wav) defining the stimulus characteristics:

Filename identifiers 

Speaker (S01 to S11).
Emotion (achievement, anger, fear, pain, pleasure, and surprise).
Emotional intensity (low, moderate, strong, peak).
Item-ID (unique integer identifier within speaker x emotion x intensity conditions) 
Folder structure

    Full set: all 1085 VIVAE files
    Core set: selected 480 VIVAE files 

    <root directory>
        |
        ├───README.md
        |
        └───Full_set
        |   ├───Achievement
        |   ├───Anger
        |   ├───Fear
        |   ├───Pain
        |   ├───Pleasure
        |   └───Surprise
        ├───Core_set
            ├───Achievement
            ├───Anger
            ├───Fear
            ├───Pain
            ├───Pleasure
            └───Surprise
               




        

## Acknowledgments:

Holz, Natalie, Larrouy-Maestri, Pauline, & Poeppel, David. (2020). The Variably Intense Vocalizations of Affect and Emotion Corpus (VIVAE) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.4066235

</br>

## Citations
**Please cite the VIVAE if it is used in your work in any form.**

Holz, Natalie, Larrouy-Maestri, Pauline, & Poeppel, David. (2020). The Variably Intense Vocalizations of Affect and Emotion Corpus (VIVAE) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.4066235


</br>

## License information


The VIVAE is released under a Creative Commons Attribution-NonCommercial 4.0 International License, CC BY-NC 4.0. 

For VIVAE usage inquiries not specified or accredited under the CC BY-NC 4.0 license, please contact us at natalie.holz@ae.mpg.de to request permission.

Publication date: October 5, 2020
Original Dataset: [VIVAE](https://zenodo.org/record/4066235#.YWcWERpByUm)

------

This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)

