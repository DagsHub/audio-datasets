**This dataset is uploaded to [DagsHub](https://dagshub.com/L-theorist/Golos), enabling you to preview (i.e. *prehear*) it before downloading.**


## Golos - Russian ASR dataset
**Note:** This is at the moment only a sample of the whole dataset: 

    train/test/crowd/0
    test
    *.jsonl
---
## General Information
Golos is a Russian corpus suitable for speech research. The dataset mainly consists of recorded audio files manually annotated on the crowd-sourcing platform. The total duration of the audio is about 1240 hours. 


For more overview see [the research article](https://dagshub.com/L-theorist/Golos/src/master/2106.10161.pdf). For a detailed account and acoustic models please consult the original [github repository](https://github.com/sberdevices/golos).

## *Folder* structure
```
.
├── test
│   ├── crowd
│   │   └── files
│   └── farfield
│       └── files
└── train
    ├── crowd
    │   ├── 0
    │   ├── 1   (not uploaded yet)
    │   ├── 2   (not uploaded yet)
    │   ├── 3   (not uploaded yet)
    │   ├── 4   (not uploaded yet)
    │   ├── 5   (not uploaded yet)
    │   ├── 6   (not uploaded yet)
    │   ├── 7   (not uploaded yet)
    │   ├── 8   (not uploaded yet)
    │   └── 9   (not uploaded yet)
    └── farfield
    ├──── 1hour.jsonl
    ├──── 10hours.jsonl
    ├──── 10min.jsonl
    ├──── 100hours.jsonl
    ├──── manifest.jsonl
```
## **Full Dataset structure**

| Domain         | Train files | Train hours  | Test files | Test hours |
|----------------|------------|--------|-------|------|
| Crowd          | 979 796    | 1 095  | 9 994 | 11.2 |
| Farfield       | 124 003    |   132.4| 1 916 |  1.4 |
| Total          | 1 103 799  | 1 227.4|11 910 | 12.6 |

---


## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a variant of <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

Please see the specific [license](https://dagshub.com/L-theorist/Golos/src/master/en_us.pdf).

## Authors and Credits

    Alexander Denisenko
    Angelina Kovalenko
    Fedor Minkin
    Nikolay Karpov


You can cite the data using the following BibTeX entry:

  @article{karpov2021golos,
    title={Golos: Russian Dataset for Speech Research},
    author={Karpov, Nikolay and Denisenko, Alexander and Minkin, Fedor},
    journal={arXiv preprint arXiv:2106.10161},
    year={2021}
  }


