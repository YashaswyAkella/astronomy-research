# J1237+3314: What Is Beside This Quasar?

An independent astronomy project by **Yashaswy Akella**.

> **Status:** Exploratory research; not peer-reviewed.
> The central measurements have not yet been independently reproduced.
> This project does not establish a new gravitational lens or a
> confirmed dual active galactic nucleus.

## The question

A known quasar has a faint neighbour in the sky.

Are they physically associated, two images created by gravitational
lensing, or unrelated objects at different distances?

This project examines public observations to investigate that question.

**The answer remains unresolved.**

## Start here

- [Plain-language HTML explainer](index.html)
- [LaTeX report source](project_report.tex)

GitHub may show the HTML source rather than the designed page.
Use the GitHub Pages website or open `index.html` in your browser.

After compiling the LaTeX report, its PDF can be added as
`project_report.pdf`.

## The two components

- **A:** the bright quasar SDSS J123704.05+331423.8,
  at redshift approximately 1.288.
- **B:** the faint optical source about 1.62 arcseconds from A.

| Component | Gaia DR3 identifier |
|---|---|
| A | `1514739204708610432` |
| B | `1514739204711602816` |

The objects and candidate pair were already catalogued.
This project did not discover them.

## What the analysis reports

### Radio–optical association

The precise position of the compact radio source JVAS B1234+335
is approximately 4.7 milliarcseconds from B's Gaia position,
compared with approximately 1.619 arcseconds from A.

This supports associating the radio emission with B's position.
It does not establish B's distance.

### Spectral feature

The DESI spectrum taken towards B contains a reported feature near
8528.6 Å.

The feature is reported:
- In the combined spectrum.
- In both individual exposures.
- Before correcting for contamination from A.
- In an additional extraction from preprocessed detector images.

These are checks using the same underlying observations.
They are not independent observational confirmation.

### Possible oxygen identification

The feature is consistent with [O II] emission at a gas redshift
of approximately 1.2872–1.2879.

Other identifications remain possible. Even if the oxygen
identification is correct, the gas may belong to A's surroundings
rather than to B.

## What is not established

This project does not establish:
- A confirmed dual AGN.
- A secure redshift for B's compact radio nucleus.
- A definitive rejection of gravitational lensing.
- Discovery of the already known sources or pair.
- Priority for the spectral feature or its interpretation.

The radio sensitivity thresholds and spatial constraints depend
on modelling assumptions.

## Verification status

The code has undergone iterative development and static review.
That does not certify the scientific calculations.

Independent reproduction of the central measurements is not
documented in this release.

If the workflow fails to run, record the error and environment
rather than describing the release as fully verified.

## Project files

```text
index.html
README.md
project_report.tex
CITATION.cff
.gitignore

release/
├── README.md
├── requirements.txt
├── data_provenance.md
├── scripts/
├── downloads/
├── out/
└── manuscripts/
```

The corrected analysis package belongs in `release/`.
Keep its internal structure unchanged because scripts use
relative paths.

The explanatory files above do not replace the analysis scripts.

## Running the analysis

Use `release/README.md` for the intended software environment,
required inputs, and commands.

The complete release is required. Some large DESI files are
downloaded separately, and the download script does not retrieve
every required input.

A successful run demonstrates execution—not automatically correct
modelling, uncertainty coverage, or physical interpretation.

## Next useful steps

1. Independently check the spectral feature and positional association.
2. Assess instrumental and modelling limitations.
3. Check relevant previous literature.
4. Use spatially resolved observations if available.

## Data credits and permissions

The project uses public data and services including Gaia, DESI,
the DESI Legacy Imaging Surveys, JVAS, FIRST, VLASS,
the Radio Fundamental Catalog, SDSS, SIMBAD, and VizieR.
Supporting analyses use WISE and unWISE.

See the technical documentation for references and input provenance.

Original survey data retain their providers' terms and
acknowledgement requirements. A licence for the author's original
code does not relicense third-party observations.

## AI assistance

AI tools assisted with discussion, code development, code review,
and writing. This explanatory documentation was prepared with
assistance from ChatGPT (OpenAI).

AI assistance is not independent scientific validation.
The technical documentation should accurately identify other
tools used and the checks actually performed.

## Feedback

Corrections and independent reproduction attempts are welcome
through GitHub Issues.

Please identify the project version, file involved, and whether
the issue concerns execution, measurement, uncertainty, or
interpretation.

## Why share this?

An unresolved investigation can still be worth documenting.

This repository records the question, methods, reported evidence,
and limitations—not a confirmed discovery announcement.