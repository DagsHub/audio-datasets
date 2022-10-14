# FSL4-4K_User_Contributed_Loops

### Paper: [Tempo Estimation for Music Loops and a Simple Confidence Measure](https://archives.ismir.net/ismir2016/paper/000195.pdf)
### DagsHub Repository: [FSL4-4K_User_Contributed_Loops](https://dagshub.com/Rutam21/FSL4-4K_User_Contributed_Loops)

![DagsHub Hacktoberfest Cover](https://user-images.githubusercontent.com/66431403/192983164-b3d6d556-ac69-4fb8-8aef-726a4386406a.png)

## About

The FSL4 dataset contains ~4000 user-contributed loops uploaded to Freesound. Loops were selected by searching Freesound for sounds with the query terms loop and bpm, and then automatically parsing the returned sound filenames, tags and textual descriptions to identify tempo annotations made by users. For example, a sound containing the tag 120bpm is considered to have a ground truth of 120 BPM.

## Dataset

The dataset contains a number of raw audio files in different formats (wav, aif, flac, mp3 and ogg), and a metadata.json file with metadata about the audio files. Audio files are all contained in the same directory and use Freesound IDs as filenames (e.g. 1234.wav, where the Freesound ID is 1234). The metadata.json file contains a dictionary with keys corresponding to Freesound IDs (note that the .json extension had to be removed because of Zenodo's limitations). Tempo (BPM) annotations can be found in the annotations property of each entry in the dictionary.

The BPM ground truth collected from user annotations is typically correct, but it was observed that around 5% of the cases could be wrong or very ambiguous annotations.

> Note that even though the dataset metadata is released under CC-BY-4.0 license, the individual audio files have their own Creative Commons licenses. Licenses for these files are listed both in the metadata.json and about.txt  files.

## Citation

```
This dataset is part of the publication:
	Font, F., & Serra, X. (2016). "Tempo Estimation for Music Loops and a Simple 
	Confidence Measure". In Proceedings of the Int. Conf. on Music Information Retrieval (ISMIR).
```
