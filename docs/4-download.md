# Get the MELI corpus 

## Download

MELI is available through the UBC Research Data Collection via Scholars Portal Dataverse. You can access MELI from the button below. 

MELI is freely available under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). That means you can use, copy, share, and adapt it, as long as you don't release your adaptation with additional restrictions, *and* you cite the corpus.

<!-- <div align="center">
  <a href="https://doi.org/10.5683/SP3/5WMRUO" style="
    background-color: #5b9bd5;
    color: white;
    padding: 10px 20px;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 600;
    display: inline-block;
  ">
    Download MELI
  </a>
</div> -->

<div style="
  border: 1.5px solid #5b9bd5;
  background-color: #f4f8fc;
  padding: 20px;
  border-radius: 8px;
  max-width: 650px;
  margin: 20px auto;
  text-align: center;
">

  <p style="margin-top: 0;">
    💐 As you explore the corpus, I hope you’ll take a moment to appreciate the people behind the data: their willingness to share their voices, perspectives, and stories. Please engage with the material with care and curiosity.
  </p>

  <label style="display: inline-flex; align-items: center; gap: 8px; margin-top: 10px;">
    <input type="checkbox" id="ack">
    I agree to engage with MELI with care and curiosity.
  </label>

  <br><br>

  <a id="downloadBtn" href="https://doi.org/10.5683/SP3/5WMRUO" style="
    background-color: #5b9bd5;
    color: white;
    padding: 10px 20px;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 600;
    display: inline-block;
    pointer-events: none;
    opacity: 0.5;
  ">
    Download MELI
  </a>

</div>

<script>
document.getElementById('ack').addEventListener('change', function() {
  const btn = document.getElementById('downloadBtn');
  if (this.checked) {
    btn.style.pointerEvents = 'auto';
    btn.style.opacity = '1';
  } else {
    btn.style.pointerEvents = 'none';
    btn.style.opacity = '0.5';
  }
});
</script>

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

