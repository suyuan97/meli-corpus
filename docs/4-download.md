# Get the MELI corpus 

## Download

MELI is available through the UBC Research Data Collection via Scholars Portal Dataverse. You can access MELI from the button below. 

MELI is freely available under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). That means you can use, copy, share, and adapt it, as long as you don't release your adaptation with additional restrictions, *and* you cite the corpus.

<div align="center"><button class="button" onclick="https://doi.org/10.5683/SP3/5WMRUO">Download MELI</button></div>
<br>

## Citation

We prefer that you cite the corpus directly:

```text
@data{liubabel2026meli,
	author = {Liu, Suyuan and Babel, Molly},
	publisher = {Scholars Portal Dataverse},
	title = {MELI: Mandarin-English Language Interview},
	year = {2026},
	version = {Version 1},
	doi = {10.5683/SP3/5WMRUO},
	url = {https://doi.org/10.5683/SP3/5WMRUO}
} 
```

<!-- But if you can't do that, then you can also cite the following paper: -->

<!-- ```text
@inproceedings{liubabel2026lrec,
    title = {SpiCE: A new open-access corpus of conversational bilingual speech in Cantonese and English},
    author = {Johnson, Khia A. and Babel, Molly and Fong, Ivan and Yiu, Nancy},
    booktitle = {Proceedings of the 12th Language Resources and Evaluation Conference},
    month = may,
    year = {2020},
    address = {Marseille, France},
    publisher = {European Language Resources Association},
    url = {https://www.aclweb.org/anthology/2020.lrec-1.503},
    pages = {4089--4095},
    language = {English},
    ISBN = {979-10-95546-34-4},
}
``` -->

<!-- ```text
@misc{liu2026introducingmelimandarinenglishlanguage,
      title={Introducing MELI: the Mandarin-English Language Interview Corpus}, 
      author={Suyuan Liu and Molly Babel},
      year={2026},
      eprint={2603.27043},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2603.27043}, 
}
``` -->

## What's in the download?

The download comes with:

- A `README.md` file
- Tabular metadata including language background
- Out-of-vocabulary (OOV) files used in the forced alignment process
- A copy of this documentation
- 2 languages x 51 talkers = 102 `.wav` files (stereo, 16-bit, 44.1 kHz)
- 2 languages x 51 talkers = 102 `.TextGrid` files (each with 4 tiers: task, utterance-corrected, word, phone)
- 1 map x 51 talkers = 51 `.png` files from the draw-a-map task

The `wav` and `textgrid` files have a consitent format. For example, `F01A_man` would correspond to the following:

> | Text                | What it means    | Other categories |
> | :------------------ | :--------------- | :--------------- |
> | `F`                | Female           | `M` = Male      |
> | `01`                | Year of Birth              | varies `(19)89`-`(20)05` |
> | `man`         | Language         | `eng`        |

<br>
Unique participant IDs are made up of the first four characters. In this example, that would be `F01A`. This ID is used in the language background summary. 

## Ethics

The corpus was developed in accordance with the [University of British Columbia Behavioural Research Ethics Board](https://ethics.research.ubc.ca/behavioural-research-ethics) (H23-03205). 

## Funding

MELI was funded by Arts Graduate Research Awards to Suyuan Liu and by a [Social Sciences and Humanities Research Council of Canada (SSHRC)](https://www.sshrc-crsh.gc.ca/) Insight Grant to Molly Babel.

