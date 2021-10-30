**This dataset is uploaded to [DagsHub](https://dagshub.com/L-theorist/Deeply_Nonverbal_Vocalization_Dataset), enabling you to preview (i.e. *prehear*) it before downloading.**

# Deeply Vocal Characterizer Dataset
## Sample Dataset
---
## General Information
This dataset is a sample of the bigger corpus *The Vocal Characterizer Dataset*. The latter is <u>*__a human nonverbal vocal sound dataset__*</u> consisting of <u>*__56.7 hours__*</u> of short clips from <u>*__1419 speakers__*</u>, crowdsourced by the general public in South Korea. Also, the dataset includes metadata such as age, sex, noise level, and quality of utterance. 16 classes of Included human nonverbal sound contain <u>*__‘teeth-chattering’, ‘teeth-grinding’, ‘tongue-clicking’, ‘nose-blowing’, ‘coughing’, ‘yawning’, ‘throat clearing’, ‘sighing’, ‘lip-popping’, ‘lip-smacking’, ‘panting’, ’crying’, ‘laughing’, ‘sneezing’, ‘moaning’, and ‘screaming’.__*</u>

  **Device** | **Android phones** |
  :-:|:-:|
  **Volume** | **\~ 57 hours, ~ 70,000 utterances,<br /> ~ 18 GB, ~ 1500 speakers** |
  **Format** | **wav/h5(16/44.1kHz, 16-bit, mono)** |

The sample dataset here consists of 723 utterances (ca. 1% of the whole corpus) and is free to use under [CC BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/). For accessing the complete dataset under a more restrictive license please contact http://deeplyinc.com/us. See the [dataset description](https://dagshub.com/L-theorist/Deeply_Nonverbal_Vocalization_Dataset/src/master/Deeply%20Nonverbal%20Vocalization%20Dataset%20description_Eng.pdf) and the original [Github repository](https://github.com/deeplyinc/Nonverbal-Vocalization-Dataset) for a more detailed account.

## Structure
```

├── Nonverbal_Vocalization.json
├── coughing
├────── 0C1S_4_8_0_27_0_1_1.wav
│   ├── ...
├── crying
│   ├── 1TCO_11_10_0_20_0_0_0.wav
│   ├── ...
├── ...
├── ...
├── tongue-clicking
│   ├── 06RU_2_7_1_38_0_0_0.wav
│   ├── ...
└── yawning
    ├── 0DYI_5_10_1_12_0_1_0.wav
    ├── ...
└── Deeply\ Nonverbal\ Vocalization\ Dataset\ description_Eng.pdf
    
```

### Filename convention
{speaker_ID}\_{class}\_{trial}\_{sex}\_{age}\_{location}\_{quality}\_{noise}.wav
```
Class: {0: ‘teeth-chattering’, 1: ‘teeth-grinding’, 2: ‘tongue-clicking’, 3: ‘nose-blowing’, 
    4: ‘coughing’, 5: ‘yawning’, 6: ‘throat-clearing’, 7: ‘sighing’, 8: ‘lip-popping’, 
    9: ‘lip-smacking’, 10: ‘panting’, 11: ‘crying’, 12: ‘laughing’, 13: ‘sneezing’, 14: ‘moaning’, 15: screaming’}
Sex: {0: ‘Female’, 1: ‘Male’}
Location: {0: ‘indoor’, 1: ‘outdoor’}
Quality: {0: ‘High’, 1: ‘Low’}
Noise: {0: ‘Noiseless’, 1: ‘Noisy’}
```

## License
  <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

## Contact
Tel:   (+82) 70-7459-0704  
Web:   http://deeplyinc.com/  
Email: contact@deeplyinc.com

