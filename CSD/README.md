# CSD

> Children's Song Dataset for Singing Voice Research

Children's Song Dataset is open source dataset for singing voice research. This dataset contains 50 Korean and 50 English songs sung by one Korean female professional pop singer. Each song is recorded in two separate keys resulting in a total of 200 audio recordings. Each audio recording is paired with a MIDI transcription and lyrics annotations in both grapheme-level and phoneme-level.

## Dataset Structure

The entire data splits into Korean and English and each language splits into 'wav', 'mid', 'lyric', 'txt' and 'csv' folders. Each song has the identical file name for each format. Each format represents following information. Additional information like original song name, tempo and time signature for each song can be found in 'metadata.json'.

*    'wav': Vocal recordings in 44.1kHz 16bit wav format
*    'mid': Score information in MIDI format
*    'lyric':  Lyric information in grapheme-level
*    'txt': Lyric information in syllable and phoneme-level
*    'csv': Note onsets and offsets and syllable timings in comma-separated value (CSV) format

## Vocal Recording

While recording vocals, the singer sang along with the background music tracks. She deliberately rendered the singing in a “plain” style refraining from expressive singing skills. The recording took place in a dedicated soundproof room. Singer recorded three to four takes for each song and the best parts are combined into a single audio track. Two identical songs with different keys are discriminated by character 'a' and 'b' at the end of a filename.

## MIDI Transcription

The MIDI data consists of monophonic notes. Each note contains onset and offset times which were manually fine-tuned along with the corresponding syllable. MIDI notes do not include any expression data or control change messages because those parameters can be ambiguous to define for singing voice. Singing voice is an highly expressive sound and it is hard to define precise onset timings and pitches. We assumed one syllable matches with one MIDI note and made the following criteria to represent various expressions in singing voice.

*    A piano sound is used as a reference tone for the annotated MIDI to ensure the alignment with vocal.
*    The rising pitch at the beginning of a note is included within a single note.
*    The end of syllable is treated as the offset of a note.
*    The breathing sound during short pauses is not treated as note onset or offset.
*    Vibrations are treated as a single sustaining note.
*    If a syllable is rendered with several different pitches, we annotated them as separate notes.

## Lyric Annotation

Text files in the 'lyric' folder contains raw text for corresponding audio and the 'txt' folder contains phoneme-level lyric representation. The phoneme-level lyric representation is annotated in a special text format. Phonemes in a syllable are tied with underbar('_') and syllables are separated with space(' '). Each phonemes are annotated based on the international phonetic alphabet (IPA) and romanized symbols are used to annotate IPA symbols. *You can find romanized IPA symbols and more detailed information in this [repository](https://github.com/emotiontts/emotiontts_open_db/tree/master/Dataset/CSD).*

## License

This dataset was created by the KAIST [Music and Audio Computing Lab](http://mac.kaist.ac.kr/) under Industrial Technology Innovation Program (No. 10080667, Development of conversational speech synthesis technology to express emotion and personality of robots through sound source diversification) supported support by the Ministry of Trade, Industry & Energy (MOTIE, Korea).

CSD is released under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0). **It is provided primarily for research purposes and it is prohibited to be used for commercial purposes. When sharing your result based on CSD, any act that defames the original singer is strictly prohibited.**

For more details, we refer to the following publication. We would highly appreciate if publications partly based on CSD quote the following publication:

> Choi, S., Kim, W., Park, S., Yong, S., & Nam, J. (2020). [Children’s Song Dataset for Singing Voice Research](https://program.ismir2020.net/static/lbd/ISMIR2020-LBD-435-abstract.pdf). 21th International Society for Music Information Retrieval Conference (ISMIR).

We are interested in knowing if you find CSD useful. If you use CSD please email us at [kaist.mac@gmail.com](mailto:kaist.mac@gmail.com) and tell us about your research.

**Source of the database [CSD](https://zenodo.org/record/4785016#.YWv-_Rx8rIX)**  
**Check this database in [Dagshub](https://dagshub.com/kinkusuma/children-song-dataset)**
