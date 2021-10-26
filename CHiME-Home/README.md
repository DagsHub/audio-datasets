# CHiME-Home

The CHiME-Home dataset is a collection of annotated domestic environment audio recordings.

![image](https://dagshub.com/kingabzpro/CHiME-Home/raw/master/asset/image.jpg)

The audio recordings and annotations included in this archive form the CHiME-Home dataset. To cite this dataset, please use the reference provided at the end of this document. Please refer to the same publication for a more detailed description of the dataset.

The CHiME-Home dataset is a collection of annotated domestic environment audio recordings. The audio recordings were originally made for the CHiME project (cf. Christensen et al., 2010; Barker et al., 2013). In the CHiME-Home dataset, 4-second audio chunks are each associated with multiple labels, based on a set of 7 labels associated with sound sources in the acoustic environment. For a total of 6137 4-second audio chunks, there are 3 sets of multi-label annotations. A subset of the 6137 chunks (1946 chunks) is further specified, for which annotators' label assignments agree strongly (cf. Foster et al., 2015). For clearer distinction, please refer to the 2762-chunk dataset as CHiME-Home-refine; correspondingly please refer to the 6137-chunk dataset as CHiME-Home-raw.

**The similar version of dataset is uploaded to DagsHub: [CHiME-Home](https://dagshub.com/kingabzpro/CHiME-Home), enabling you to preview the dataset before downloading it.**

**Please note:** As reported in Foster et al. (2015), a proportion of the aforementioned data were withheld as evaluation data for the DCASE 2016 challenge (see www.cs.tut.fi/sgn/arg/dcase2016/). This version of the CHiME-Home dataset includes the DCASE 2016 evaluation data and thus subsumes the version originally released which consisted of 4378 audio chunks and annotations. Please further note that the paper erroneously reported the total number of chunks as 6138 (instead of 6137), with the number of withheld chunks reported as 1760 (instead of 1759).

## Dataset split

Dataset was divided into two parts so that it can be viewed in DAGsHub. Just combine both **chunks1** and **chunks2** -> **chunks** if you want to use it properly. 

Directory structure and file descriptions
-------------------

The chunks/ directory contains a CSV file for each of the annotated 4-second audio chunks. The name of the CSV file uniquely identifies the chunk. Each of the CSV files contains the following fields:

segmentname: The name of the audio segment from which the chunk was obtained. 
chunknumber: The offset within the audio segment from which the chunk was obtained, in 4-second units.
framestart: The offset within the audio segment from which the chunk was obtained, in frames.
annotation_a1: The chunk's annotation string, as given by annotator A1.
annotation_a2: The chunk's annotation string, as given by annotator A2.
annotation_a3: The chunk's annotation string, as given by annotator A3.
session_a1: The annotation session during which the chunk was annotated by A1.
session_a2: The annotation session during which the chunk was annotated by A2.
session_a3: The annotation session during which the chunk was annotated by A3.
majorityvote: The chunk's annotation string, obtained by applying a majority vote about the presence of each label.
chunkname: The chunk's unique identifier, obtained from the fields segmentname and chunknumber.

In the chunks/ directory, each chunk is represented at the sampling rate 48kHz, at 16 bits per sample and in stereo. In addition, chunks are provided at a sampling rate of 16kHz as monophonic recordings. For each chunk, these two recording versions are distinguished using suffixes ".NkHz" preceding the ".wav" filename extension, where N is the sampling rate in kHz. For the DCASE 2016 challenge (see www.cs.tut.fi/sgn/arg/dcase2016/), evaluations were based on the monophonic recordings sampled at 16kHz.

The top-level directory contains the following CSV files listing audio chunks:

development_chunks_raw.csv: Chunks included in the original CHiME-Home-raw dataset (4378 chunks, see paper for further details)
development_chunks_refined.csv: Chunks included in the original CHiME-Home-refine dataset (1946 chunks with strong annotator agreement, see paper for further details)
(These data were previously used as part of a `development' dataset in the DCASE 2016 challenge; see www.cs.tut.fi/sgn/arg/dcase2016/task-audio-tagging)

evaluation_chunks_raw.csv: Chunks extending the original CHiME-Home-raw dataset (1759 chunks)
evaluation_chunks_refined.csv: Chunks extending the original CHiME-Home-refine dataset (816 chunks with strong annotator agreement)
(The evaluation_chunks_refined data were used as an `evaluation' dataset in the DCASE 2016 challenge)

In addition, the top-level directory contains a CSV file defining a partition for 5-fold cross-validation:

development_chunks_refined_crossval_dcase.csv: Chunks included in the DCASE 2016 `development' subset of CHiME-Home-refine, partitioned into 5 folds)

Method for resampling recordings
-------------------

Monophonic recordings at 16kHz were obtained by downsampling from 48kHz using SoX version 14.3.2 (see sox.sourceforge.net). SoX was invoked as:

sox $infile -c 1 $outfile rate -v 16k remix 0 1

How to cite
-------------------

P. Foster, S. Sigtia, S. Krstulovic, J. Barker, M. D. Plumbley. "CHiME-Home: A Dataset for Sound Source Recognition in a Domestic Environment," in Proceedings of the 11th Workshop on Applications of Signal Processing to Audio and Acoustics (WASPAA), 2015.

## License

This work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/3.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.                                            

Copyright for annotation data (c) 2015 Queen Mary University of London.
Copyright for audio recordings (c) 2010 University of Sheffield.

## History

- Version 0.9.4 (2015/07/18): Initial release version
- Version 0.9.5 (2016/02/04): Make chunks available at multiple sampling rates and include partition for 5-fold cross-validation using CHiME-Home-refine 
- Version 0.9.6 (2016/06/01): Incorporate DCASE 2016 evaluation chunks
- Version 0.9.7 (2016/09/08): Incorporate annotations for DCASE 2016 evaluation chunks

---

**Version 0.9.7**

**Original Dataset:** [CHiME-Home](https://archive.org/details/chime-home)

**DAGsHub Dataset:** [kingabzpro/CHiME-Home](https://dagshub.com/kingabzpro/CHiME-Home)

**Photo** by <a href="https://unsplash.com/@insolitus?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Rowan Heuvel</a> on <a href="https://unsplash.com/s/photos/home?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

------

*This open source contribution is part of [DagsHub x Hacktoberfest](https://dagshub.com/blog/hacktoberfest-x-dagshub-2/)*