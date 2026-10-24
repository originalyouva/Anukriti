# Anukriti: Virtual Trials for Real Patients

**An AI-accelerated pharmacogenomic simulator for antiplatelet therapy in Indian populations.**

Anukriti is an interactive in-silico trial simulator that shows what a standard clopidogrel dose does across different populations, with a focus on CYP2C19 variation in Indian patients. It runs entirely in the browser and uses no patient data.

> **Disclaimer:** Anukriti is an educational tool. It is not clinical evidence and cannot recommend treatment for an individual patient.

## Run it

The site is a single self-contained file with libraries and fonts embedded, so it works offline.

- **Locally:** download the repository and open [`index.html`](index.html) in any modern browser.
- **GitHub Pages:** https://originalyouva.github.io/Anukriti/

## Abstract

Clopidogrel is widely prescribed after heart attack and stenting, yet it works only after the liver enzyme CYP2C19 converts it into its active form. Genetic variants that impair this enzyme are common in South Asians: in one published South Indian coronary cohort, about two-thirds of patients were intermediate or poor metabolizers, and 31% still showed high platelet reactivity despite treatment. Standard dosing, however, is largely shaped by evidence from populations with different genetic profiles, and few accessible tools show what a standard dose means for Indian patients.

This project presents an interactive in-silico trial simulator. It generates thousands of virtual patients whose CYP2C19 genotypes are drawn from published population frequencies, applies a published population pharmacokinetic-pharmacodynamic model to predict platelet reactivity, and runs the same virtual trial on different populations side by side. A machine-learning surrogate, trained on the simulation's own outputs, returns results instantly as users adjust patient and population settings, while explainable-AI attribution shows which genetic and clinical factors drive inadequate response. Monte Carlo simulation expresses uncertainty in every result. With one switch, users can apply genotype-guided therapy in line with the CPIC guideline, under which intermediate and poor metabolizers receive an alternative antiplatelet agent, and watch the share of inadequately treated patients change.

The application runs in a web browser and uses no patient data. The surrogate will be validated against the mechanistic model, and the mechanistic model against published outputs. Every model, dataset and guideline will be disclosed. Stated limitations: the surrogate inherits the simulator's assumptions, the simulator is not clinical evidence, its parameters derive from limited cohorts, and it cannot recommend treatment for an individual patient. It is intended for education and for identifying where prospective Indian studies and genotype testing matter most.

**Keywords:** Artificial intelligence; in-silico clinical trials; pharmacogenomics; CYP2C19; explainable AI; precision medicine.

The original abstract document is in [`docs/Anukriti-Abstract.docx`](docs/Anukriti-Abstract.docx).

## Repository layout

| Path | Contents |
| --- | --- |
| `index.html` | The Anukriti website (final, offline, self-contained) |
| `docs/Anukriti-Abstract.docx` | Project abstract |
| `archive/Anukriti_draft_v1.html` | Earlier draft of the site, kept for reference (loads fonts from Google Fonts) |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Project context

Developed as a project by Sanskar.
