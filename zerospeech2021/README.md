**This dataset is uploaded to [DagsHub](https://dagshub.com/L-theorist/zerospeech2021_dataset), enabling you to preview (i.e. *prehear*) it before downloading.**

## ZeroSpeech Challenge 2021 Datasetls 
---
## General Information
Traditional speech and language technologies are trained with massive amounts of text and/or expert knowledge. This is not sustainable: the majority of the world’s languages do not have reliable textual or expert resources. Even in high resourced languages, there is a large domain mismatch between oral and written uses of language.

But infants learn to speak their native language, spontaneously, from raw sensory input, without supervision from text or linguists. It should be possible to do the same in machines!

The ultimate goal of the “Zero Resource Speech Challenge” 1 is to construct a system that learn an end-to-end Spoken Dialog (SD) system, in an unknown language, from scratch, using only raw sensory information available to an early language learner.


For a more detailed account and the competition timeline see [here](https://zerospeech.com/2021/index.html). For an overview of previous competitions see the [challenge website](https://zerospeech.com).

## Structure
```

├── lexical
│   ├── dev
├──────── aAAfmkmQpVz.wav
│   ├──── ...
│   └── test
├──────── aaaDSGZhrtbq.wav
│   ├──── ...
├── phonetic
│   ├── dev-clean
├──────── 84-121123-0000.wav
│   ├──── ...
│   ├── dev-other
├──────── 116-288045-0000.wav
│   ├──── ...
│   ├── test-clean
├──────── 61-70968-0000.wav
│   ├──── ...
│   └── test-other
├──────── 367-130732-0000.wav
│   ├──── ...
├── semantic
│   ├── dev
│   │   ├── librispeech
├──────────── aaRpeKDRbj.wav
│   ├──────── ...
│   │   └── synthetic
├──────────── aAbcsWWKCz.wav
│   ├──────── ...
│   │   └── gold.csv
│   │   └── pairs.csv
│   └── test
│       ├── librispeech
├──────────── AabWUdQiJx.wav
│   ├──────── ...
│       └── synthetic
├──────────── aaEGIphSpE.wav
│   ├──────── ...
└── syntactic
│   ├── dev
├──────────── aaacEBDmoCU.wav
│   ├──────── ...
│   └── test
├──────────── aAAAZvtMsGyf.wav
│   ├──────── ...

    
```

## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

## Authors and Credits
Challenge Organizing Committee
https://zerospeech.com/2021/#challenge-organizing-committee

The dataset contains pieces of the LibriSpeech dataset released under a
Creative Commons Attribution 4.0 International License (LibriSpeech (c) 2014
by Vassil Panayotov):

  phonetic/*.wav
  semantic/{dev,test}/librispeech

