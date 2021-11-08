# MS-SNSD

![abc](https://images.unsplash.com/photo-1611532736579-6b16e2b50449?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1126&q=80)
credit: [Kelly Sikkema](https://unsplash.com/@kellysikkema)

The dataset is posted to [DagsHub](https://dagshub.com/hazalkl/MS-SNSD), where you may preview it before downloading it.

### About:
This dataset contains a large collection of clean speech files and variety of environmental noise files in .wav format sampled at 16 kHz.
The main application of this dataset is to train Deep Neural Network (DNN) models to suppress background noise. But it can be used for other audio and speech applications.
We provide the recipe to mix clean speech and noise at various signal to noise ratio (SNR) conditions to generate large noisy speech dataset.
The SNR conditions and the number of hours of data required can be configured depending on the application requirements.
This dataset will continue to grow in size as we encourage researchers and practitioners to contribute to this dataset by adding more clean speech and noise clips.
This dataset will immensely help researchers and practitioners in accademia and industry to develop better models.
We also provide test set that is different from training set to evaluate the developed models.

### Structure:

The audio files are in `.wav` format and sampled at `16 kHz`


### Citation:
```
@article{reddy2019scalable,
  title={A Scalable Noisy Speech Dataset and Online Subjective Test Framework},
  author={Reddy, Chandan KA and Beyrami, Ebrahim and Pool, Jamie and Cutler, Ross and Srinivasan, Sriram and Gehrke, Johannes},
  journal={Proc. Interspeech 2019},
  pages={1816--1820},
  year={2019}
}
```

## Dataset licenses
MICROSOFT PROVIDES THE DATASETS ON AN "AS IS" BASIS. MICROSOFT MAKES NO WARRANTIES, EXPRESS OR IMPLIED, GUARANTEES OR CONDITIONS WITH RESPECT TO YOUR USE OF THE DATASETS. TO THE EXTENT PERMITTED UNDER YOUR LOCAL LAW, MICROSOFT DISCLAIMS ALL LIABILITY FOR ANY DAMAGES OR LOSSES, INLCUDING DIRECT, CONSEQUENTIAL, SPECIAL, INDIRECT, INCIDENTAL OR PUNITIVE, RESULTING FROM YOUR USE OF THE DATASETS.

The datasets are provided under the original terms that Microsoft received such datasets. See below for more information about each dataset.

The datasets used in this project are licensed as follows:
1. Clean speech: 
* PTDB-TUG: Pitch Tracking Database from Graz University of Technology https://www.spsc.tugraz.at/databases-and-tools/ptdb-tug-pitch-tracking-database-from-graz-university-of-technology.html; License: http://opendatacommons.org/licenses/odbl/1.0/ 
* Edinburgh 56 speaker dataset: https://datashare.is.ed.ac.uk/handle/10283/2791; License: https://datashare.is.ed.ac.uk/bitstream/handle/10283/2791/license_text?sequence=11&isAllowed=y 
2. Noise:
* Freesound: https://freesound.org/ Only files with CC0 licenses were selected; License: https://creativecommons.org/publicdomain/zero/1.0/
* Demand: https://zenodo.org/record/1227121#.XRKKxYhKiUk; License: https://creativecommons.org/licenses/by-sa/3.0/deed.en_CA
---
You may get the dataset by clicking on the [link](https://github.com/microsoft/MS-SNSD)