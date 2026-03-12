# SpiCE: Speech in Cantonese and English

A transcribed audio corpus of conversational Cantonese-English bilingual speech

*This SpiCE readme.md file was generated on 2021-05-13 by Khia A. Johnson*

This is the Speech in Cantonese and English (SpiCE) corpus. SpiCE is an audio corpus of conversational Cantonese-English bilingual speech recorded in Vancouver, Canada during 2018-2020. The corpus includes high-quality recordings of 34 early bilinguals in both English and Cantonese. Participants completed a sentence reading task, storyboard narration, and conversational interview in each language. These different speech tasks are available in a single audio file for each language for each talker. A Praat textgrid file accompanies each audio file. The textgrids provide hand-corrected orthographic transcription and phoneme-level forced-alignment in Cantonese and English. As an open-access language resource, SpiCE will promote bilingualism research for a typologically distinct pair of languages, of which Cantonese remains understudied despite there being millions of speakers around the world. The SpiCE corpus is especially well-suited for phonetic research on conversational speech, and enables researchers to study cross-language within-speaker phenomena for a diverse group of early Cantonese-English bilinguals. These are areas with few existing high-quality resources.


## General Information

1. Dataset Persistent ID: doi:10.5683/SP2/MJOXP3
2. Author Contact Information: 
	- Johnson, Khia A. (University of British Columbia, Linguistics, <khia.johnson@ubc.ca>) - ORCID: 0000-0001-6225-9446
	- Babel, Molly (University of British Columbia, Linguistics, <molly.babel@ubc.ca>) - ORCID: 0000-0003-1153-9557
3. Date of Collection: Start: 2018-11-05 ; End: 2020-03-10
4. Production Place: Vancouver, BC, Canada
5. Producer: Speech in Context Lab (Department of Linguistics, University of British Columbia) (SpeeCon) <https://speechincontext.arts.ubc.ca/>
6. Data Collectors: Yiu, Nancy & Fong, Ivan
7. Grant Information: 
	- UBC Public Scholars Initiative Award 
	- Social Sciences and Humanities Research Council: 435-2017-0136

## Sharing and Access Information

1. License: This work is licensed under a Creative Commons Attribution 4.0 International License: <http://creativecommons.org/licenses/by/4.0/>
2. Documentation: While acopy is included in this corpus download, the documentation is best viewed at: https://spice-corpus.readthedocs.io/
3. Recommended Citation: Johnson, Khia A., 2021, "SpiCE: Speech in Cantonese and English", <https://doi.org/10.5683/SP2/MJOXP3>, Scholars Portal Dataverse, V1.
4. Related Publication: Johnson, K. A., Babel, M., Fong, I., & Yiu, N. (2020). SpiCE: A New Open-Access Corpus of Conversational Bilingual Speech in Cantonese and English. Proceedings of The 12th Language Resources and Evaluation Conference, 4089–4095. issn: 2522-2686 <https://www.aclweb.org/anthology/2020.lrec-1.503/>

## Data and File Overview

### Audio and Transcription

The `cantonese/` and `english/` directories contain the main corpus data. Each directory has one `.wav` audio file and `.TextGrid` annotation file per session with the same base file name. File names provide basic information and can be parsed as follows:

`{TALKER}_{LANGUAGE}_{ORDER}_{DATE}.extension`

- TALKER:
	+ V stands for Vancouver
	+ F(emale) or M(ale) represents self-reported gender
	+ 19-34 represents the talker's age at time of recording
	+ A-E represent unique identifiers to differentiate same gender/age talkers
- LANGUAGE: The primary language of the interview is Cantonese or English
- ORDER: Of the two sessions, `I1` indicates first and `I2` second
- DATE: The date of the recording session in a YYYYMMDD format

### Language Background

The `info/participants` folder contains two tabular data files and one PDF.

- `spice-lbq-detailed.tab` provides a detailed, de-identified summary of language knowledge, proficiency, and use, in addition to demographic information
- `spice-lbq-summary.tab` is a more succinct, basic summary of participant language backgrounds
- `ubc-lbq-survey.pdf` is the Qualtrics survey that participants completed — the tabular files in this folder are based on the output from this survey


### Supplementary Information

The `info/alignment` directory contains files used for and produced by the forced alignment process with the Montreal Forced Aligner 1.0.1, including:

- Pronunciation dictionaries with `.dict` extensions
	+ English: stressed ARPABET, based on dictionary provided with Montreal Forced Aligner 1.0.1
	+ Cantonese: developed from Jyutping romanization using `pycantonese 3.2.3` <https://pycantonese.org/>
- "Out Of Vocabulary" files identifying words that were not in the pronunciation dictionarys with `oov` in the filenames (see Montreal Forced Aligner Documentation for additional information: <https://montreal-forced-aligner.readthedocs.io/>)
- Directories containing the acoustic models, `english_model` and `cantonese_model`. If used in future alignment, these folders should be compressed into `.zip` files.

The `info/documentation` folder contains a copy of the SpiCE Corpus documentation hosted at <https://spice-corpus.readthedocs.io/>, which describes the design, recording procedures, and transcription pipeline used to develop the SpiCE Corpus.