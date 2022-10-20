# WARBLRB10k-10K_Smartphone_Recording_Dataset
### Paper: [Automatic acoustic detection of birds through deep learning: the first Bird Audio Detection challenge](https://arxiv.org/pdf/1807.05812.pdf)
### DagsHub Repository: [WARBLRB10k-10K_Smartphone_Recording_Dataset](https://dagshub.com/Rutam21/WARBLRB10k-10K_Smartphone_Recording_Dataset)

![DagsHub Hacktoberfest Cover](https://user-images.githubusercontent.com/66431403/192983164-b3d6d556-ac69-4fb8-8aef-726a4386406a.png)

## About

warblrb10k is a collection of 10,000 smartphone audio recordings from around the UK, crowdsourced by users of Warblr the bird recognition app. The audio covers a wide distribution of UK locations and environments, and includes weather noise, traffic noise, human speech and even human bird imitations.

## Dataset

This repository contains two sets of data, mainly for dvelopment followed by training purposes.

### Development

**Crowdsourced dataset, UK ("warblrb10k")** - 8,000 smartphone audio recordings from around the UK, crowdsourced by users of Warblr the bird recognition app. The audio covers a wide distribution of UK locations and environments, and includes weather noise, traffic noise, human speech and even human bird imitations.

### Evaluation

**Crowdsourced dataset, UK ("warblrb10k")** - This is a held-out set of 2,000 recordings from the same conditions as the Warblr development dataset.

> Note: All these datasets are added here.

## Citation

```
@article{Stowell_2018badchj,
    Author = "Stowell, D. and Stylianou, Y. and Wood, M. and Pamu{\l}a, H. and Glotin, H.",
    title = "Automatic acoustic detection of birds through deep learning: the first Bird Audio Detection challenge",
    journal = "Methods in Ecology and Evolution",
    archiveprefix = "arXiv",
    eprint = "1807.05812",
    year = "2018",
    url = "https://arxiv.org/abs/1807.05812]",
    abstract = "Assessing the presence and abundance of birds is important for monitoring specific species as well as overall ecosystem health. Many birds are most readily detected by their sounds, and thus passive acoustic monitoring is highly appropriate. Yet acoustic monitoring is often held back by practical limitations such as the need for manual configuration, reliance on example sound libraries, low accuracy, low robustness, and limited ability to generalise to novel acoustic conditions. Here we report outcomes from a collaborative data challenge showing that with modern machine learning including deep learning, general-purpose acoustic bird detection can achieve very high retrieval rates in remote monitoring data --- with no manual recalibration, and no pre-training of the detector for the target species or the acoustic conditions in the target environment. Multiple methods were able to attain performance of around 88\% AUC (area under the ROC curve), much higher performance than previous general-purpose methods. We present new acoustic monitoring datasets, summarise the machine learning techniques proposed by challenge teams, conduct detailed performance evaluation, and discuss how such approaches to detection can be integrated into remote monitoring projects."
}
```
