# DAPS Dataset


[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4660670.svg)](https://doi.org/10.5281/zenodo.4660670)


The DAPS (Device and Produced Speech) dataset is a collection of aligned versions of professionally produced studio speech recordings and recordings of the same speech on common consumer devices (tablet and smartphone) in real-world environments. It has 15 versions of audio (3 professional versions and 12 consumer device/real-world environment combinations). Each version consists of about 4 1/2 hours of data (about 14 minutes from each of 20 speakers). Please see this paper for a detailed description of the dataset:

Gautham J. Mysore, [“Can We Automatically Transform Speech Recorded on Common Consumer Devices in Real-World Environments into Professional Production Quality Speech? - A Dataset, Insights, and Challenges”](https://ieeexplore.ieee.org/document/6981922), in the IEEE Signal Processing Letters, Vol. 22, No. 8, August 2015

The primary goal of the dataset is to help develop methods to automatically convert real-world device recordings into professional sounding recordings. It can be also used for various other applications like voice conversion, traditional speech enhancement, and automatic production of studio recordings.

Audio Files Included
--------------------

Each version contains 100 wave files - 20 speakers reading 5 scripts each (about 14 minutes of data per speaker). We provide a separate folder for each version.

-----

### Description of Studio Recordings 

The versions are:

- cleanraw - Original clean studio recording, which includes speech as well as non-speech sounds such as breaths and mouth sounds.

- clean - A version of cleanraw with most of the non-speech sounds carefully removed by a professional sound engineer.

- produced - A version of clean with effects and processing such as EQ and compression applied by the same sound engineer. This is the final studio version.

The file naming convention is:
speaker_script_version.wav

For example, f2_script4_produced.wav, is the professionally produced version of the second female speaker reading the fourth script .


-----

### Description of Device Recordings  

Devices:
  
- ipad - An iPad Air was placed on a stand to simulate a person holding it. This recording was done in all environments.

- ipadflat - An iPad Air was placed flat on a table. This recording was done in two environments.

- iphone - An iPhone 5S was placed on a stand to simulate a person holding it. This recording was done in three environments.

Environments:  

- office1 - more reverberant office

- office2 - less reverberant office

- confroom1 - smaller conference room

- confroom2 - larger conference room

- livingroom1 - relatively reverberant living room with occasional traffic noise from outside

- bedroom1 - bedroom with occasional traffic noise from outside

- balcony1 - balcony with heavy traffic noise (this was used as a stress test and has significantly higher noise than all other environments)


The file naming convention is:  
speaker_script_device_room.wav

For example, m5_script1_ipad_office1.wav, is the iPad recording in the first office of the fifth male speaker reading the first script.

-----

### Sample files 

In the sample folder, we provide all versions of a single speaker reading a single script. It is a quick way to listen to the differences between versions. We also provide an Adobe Audition session file with all sample files for convenience.



Additional Files Included
------------------------

The folder called supplementary_files contains the actual scripts read by the speakers as well as a set of Matlab files to assist in creating new device recordings.



Please Acknowledge DAPS in Academic Research
----------------------------------------------------

When DAPS is used for academic research, we would highly appreciate it if scientific publications of works partly based on the DAPS dataset cite the following publication:

Gautham J. Mysore, “Can We Automatically Transform Speech Recorded on Common Consumer Devices in Real-World Environments into Professional Production Quality Speech? - A Dataset, Insights, and Challenges”, in the IEEE Signal Processing Letters, Vol. 22, No. 8, August 2015



License
----------------------------------------------------

The DAPS dataset is licensed under Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)

----------------------------------------------------

**Check this dataset in [dagshub](https://dagshub.com/kinkusuma/daps-dataset)**
