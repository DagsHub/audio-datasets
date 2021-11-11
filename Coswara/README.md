
# Coswara-Data

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

Project Coswara by Indian Institute of Science (IISc) Bangalore is an attempt to build a diagnostic tool for COVID-19 detection using the audio recordings such as breathing, cough and speech sounds of an individual. Currently, the project is in the data collection stage through crowdsourcing. To contribute your audio samples, please go to Project Coswara(https://coswara.iisc.ac.in/). The exercise takes 5-7 minutes.

<strong>What am I looking at?</strong>
This github repository contains the raw audio data collected through https://coswara.iisc.ac.in/ . Every participant contributes nine sound samples. You can read the paper: [Coswara - A Database of Breathing, Cough, and Voice Sounds for COVID-19 Diagnosis](https://arxiv.org/abs/2005.10548) to know more about the dataset. Note that the dataset size has increased since this paper came out. We also maintain a (less frequently updated) blog [here](https://iiscleap.github.io/coswara-blog/coswara/2020/11/23/visualize_coswara_data_metadata.html).

<strong>What is the structure of the repository?</strong>
Each folder contains metadata and audio recordings corresponding to contributors. The folder is compressed. To download and extract the data, you can run the script `extract_data.py`

<strong>What are the different sound samples?</strong>
Sound samples collected include breathing sounds (fast and slow), cough sounds (deep and shallow), phonation of sustained vowels (/a/ as in made, /i/,/o/), and counting numbers at slow and fast pace. Metadata information collected includes the participant's age, gender, location (country, state/ province), current health status (healthy/ exposed/ positive/recovered) and the presence of comorbidities (pre-existing medical conditions).

<strong>Can I see the metadata before downloading whole repository?</strong>
Yes. The file `combined_data.csv` contains a summary of metadata. The file `csv_labels_legend.json` contains information about the columns present in `combined_data.csv`.

<strong>How to cite this dataset in your work?</strong>
Great to know you found it useful. You can cite the paper: Coswara - A Database of Breathing, Cough, and Voice Sounds for COVID-19 Diagnosis (https://arxiv.org/abs/2005.10548)

<details><summary><strong>What is the count of participants in each folder?</strong></summary>

- 2020-04-13 contains 76 samples.
- 2020-04-15 contains 161 samples. 
- 2020-04-16 contains 197 samples.
- 2020-04-17 contains 168 samples.
- 2020-04-18 contains 46 samples. 
- 2020-04-19 contains 32 samples.
- 2020-04-24 contains 28 samples.
- 2020-04-30 contains 23 samples.
- 2020-05-02 contains 155 samples.
- 2020-05-04 contains 81 samples.
- 2020-05-05 contains 14 samples.
- 2020-05-25 contains 54 samples.
- 2020-06-04 contains 20 samples.
- 2020-07-07 contains 42 samples.
- 2020-07-20 contains 21 samples.
- 2020-08-03 contains 29 samples.
- 2020-08-14 contains 83 samples.
- 2020-08-20 contains 48 samples.
- 2020-08-24 contains 19 samples.
- 2020-09-01 contains 24 samples.
- 2020-09-11 contains 16 samples.
- 2020-09-19 contains 32 samples.
- 2020-09-30 contains 26 samples.
- 2020-10-12 contains 18 samples.
- 2020-10-31 contains 29 samples.
- 2020-11-30 contains 17 samples.
- 2020-12-21 contains 27 samples.
- 2021-02-06 contains 18 samples.
- 2021-04-06 contains 66 samples.
- 2021-04-19 contains 35 samples.
- 2021-04-26 contains 41 samples.
- 2021-05-07 contains 54 samples.
- 2021-05-23 contains 31 samples.
- 2021-06-03 contains 42 samples.
- 2021-06-18 contains 56 samples.
- 2021-06-30 contains 67 samples.
- 2021-07-14 contains 52 samples.
- 2021-08-16 contains 82 samples.
- 2021-08-30 contains 64 samples. 
- 2021-09-14 contains 37 samples.
- 2021-09-30 contains 103 samples.

Each folder also has a CSV file which contains metadata of each sample (that is, participant).


</details>

## Project Phases
The word **Coswara** is an amalgamation of Co (from corona) and Swara (sound in sanskrit). The project is being pursued in three stages:

### Data Collection
We aim at creating a dataset composed of voice samples from healthy individuals, and those with COVID-19 infection. The data is collected using a web and mobile application. Voice samples collected include breathing sounds (fast and slow), cough sounds (deep and shallow), phonation of sustained vowels (/a/ as in made, /i/,/o/), and counting numbers at slow and fast pace. Metadata information collected includes the participant's age, gender, location (country, state/ province), current health status (healthy/ exposed/ cured/ infected) and the presence of comorbidities (pre-existing medical conditions).

No personally identifiable information is collected, and the data collection respects the privacy of the contributors. The data is also anonymized during storage itself. All the collected data will be available updated here on a daily basis.

### Modelling
The collected data will be analysed using signal processing and machine learning techniques. The goal is to build mathematical models aiding identification of ‘infection prints’ from voice samples. This stage is a work-in-progress while we create the dataset.

We also aim at releasing the collected dataset in a structured form openly via a Github platform. This is to pool effort from the larger research community to contribute in making point-of-care diagnosis a reality soon.

### Diagnostic Tool
We aim to release the diagnosis tool as a web/mobile application. Similar to the dataset creation stage, the application requests for recording the voice samples, and preferably provides a score indicating the probability of COVID-19 infection. The final deployment of the tool is subject to validation with clinical findings, and authorization/approval from competent authorities.

Given the highly simplistic and cost effective nature of this diagnosis approach, we hypothesize that even a partial success of the tool would enable a massive deployment as a first line of diagnosis for the pandemic. The potential diagnostic tool will not replace chemical testing but merely supplement the existing testing methods.






## <strong>Can I know the individuals maintaining this project?</strong>
Yes, we are a team of Professors, PostDocs, Engineers, and Research Scholars affiliated with the Indian Institute of Science, Bangalore (India). [Sriram Ganapathy](http://leap.ee.iisc.ac.in/sriram/), Assistant Professor, Dept. Electrical Engineering, IISc is the Principal Investigator of this project.

Current Members: Debarpan Bhattachrya, Debottam Dutta, Neeraj Kumar Sharma, Prasanta Kumar Ghosh, Srikanth Raj Chetupalli, Sriram Ganapathy

Past Members: Anand Mohan, Ananya Muguli, Prashant Krishnan, Rohit Kumar, Shreyas Ramoji

---

The DAGshub repository is [here](https://dagshub.com/CyberFlame/Coswara-Data)
This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)
