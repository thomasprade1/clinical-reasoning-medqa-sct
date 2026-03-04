# clinical-reasoning-medqa-sct

# Supplementary Material – Benchmarking and Evaluating Clinical Reasoning

This repository contains supplementary material for the preprint "Benchmarking 
Clinical Reasoning in Large Language Models: A Comparative Assessment Study"

Medical University of Vienna, Institute for Artificial Intelligence

> Preprint: [link to be added]
---

## Overview

This study compares LLM performance, uncertainty characteristics and clinical
reasoning qualities across two medical benchmarks with fundamentally different
assessment approaches: MedQA-USMLE, a knowledge-based multiple-choice benchmark
and the public subset of SCT-Bench, which evaluates clinical reasoning and probabilistic 
thinking under uncertainty. Baseline and chain-of-thought (CoT) prompting are contrasted across
sampled responses, examining how prompted reasoning strategies affect model
behaviour differently depending on the assessment format.

A central part of this work is the design of structured CoT prompt templates that
instruct the model to apply cognitive clinical reasoning strategies drawn from the
medical cognition literature (Cooper & Frain, 2017), and the subsequent evaluation
of whether and how these strategies are employed across both benchmark formats.

---

## Repository Contents

## Repository Contents

- **notebooks** – Jupyter notebooks for model querying and data analysis
- **prompts** – CoT clinical reasoning instruction prompt templates for MedQA-USMLE and
  SCT-Bench
- **data** – benchmark datasets as obtained from their original sources
- **results** – per-question output files including full model responses, ratings,
  uncertainty scores, reasoning strategy labels and question-level statistics

---

## Datasets

If you use the datasets provided here, please cite the original contributors:

**MedQA-USMLE** is a publicly available dataset of USMLE multiple-choice
questions introduced by Jin et al. (2021). The test split comprises 1,273
four-option questions sourced from real US medical licensing examinations.
Original dataset: https://github.com/jind11/MedQA

**SCT-Bench** is a Script Concordance Testing benchmark introduced by McCoy et al.
This repository includes the publicly available subset. The full benchmark, original evaluation 
framework, and query code template are available at: https://github.com/SCT-Bench/sctpublic

---

## Requirements

Dependencies are listed in `requirements.txt`. An LLM endpoint API key is
required to re-run the querying notebooks. Analysis notebooks can be run
independently on the provided or newly generated results (response) files.

---

## Citation

Any research building on or adjacent to the ideas presented in this work should
cite the corresponding preprint:

---

## Acknowledgements

SCT-Bench data query code template adapted from McCoy et al.'s public
repository. MedQA-USMLE data from Jin et al. This work was conducted at the
Institute for Artificial Intelligence, Medical
University of Vienna under the supervision of Priv.Doz. Mag. Dr. Matthias Samwald.

---

## References

Cooper N, Frain J (eds.). *ABC of Clinical Reasoning*. First Edition.
Chichester: John Wiley & Sons; 2017.
