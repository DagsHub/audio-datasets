# The Flickr 8k Audio Caption Corpus

If you use this data, please cite

- D. Harwath and J. Glass, "Deep Multimodal Semantic Embeddings for Speech and Images," 2015 IEEE Automatic Speech Recognition and Understanding Workshop, pp. 237-244, Scottsdale, Arizona, USA, December 2015 [(PDF)](https://groups.csail.mit.edu/sls/publications/2015/Harwath_ASRU-15.pdf)

as well as the original Flickr 8k text caption corpus:

- M. Hodosh, P. Young and J. Hockenmaier (2013) "Framing Image Description as a Ranking Task: Data, Models and Evaluation Metrics", Journal of Artificial Intelligence Research, Volume 47, pages 853-899
https://www.jair.org/index.php/jair/article/view/10833/25854

You can download the original Flickr 8k corpus of text captions here:
https://forms.illinois.edu/sec/1713398

**The dataset is uploaded to DagsHub: [Flickr-Audio-Caption-Corpus](https://dagshub.com/michizhou/Flickr-Audio-Caption-Corpus), which allows you to preview parts of the dataset before downloading it.**

This data is distributed under the Creative Commons Attribution-ShareAlike (CC BY-SA) license.

## Brief description of datasets

Here is a brief description of what is included in the Flickr 8k audio data:

The wavs/ directory contains 40,000 spoken audio captions in .wav audio format, one for each caption included in the train, dev, and test splits in the original Flickr 8k corpus (as defined by the files Flickr_8k.trainImages.txt, Flickr_8k.devImages.txt, and Flickr_8k.testImages.txt)

The audio is sampled at 16000 Hz with 16-bit depth, and stored in Microsoft WAVE audio format

The file wav2capt.txt contains a mapping from the .wav file names to the corresponding .jpg images as well as caption number. The .jpg file names and caption numbers can then be mapped to the caption text via the Flickr8k.token.txt file from the original Flickr 8k corpus.

The file wav2spk.txt contains a mapping from the .wav file names to its speaker. Each unique speaker is numbered consecutively from 1 to 183 (the total number of unique speakers).

## Data downloads

Flickr Audio Corpus (4.2 GB): [Download gzip'd tar file](https://groups.csail.mit.edu/sls/downloads/flickraudio/downloads/flickr_audio.tar.gz)

MD5 checksum: 9d078f1f150c26e864aa64d1d733779a

---

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*