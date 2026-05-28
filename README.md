Chapter 99: chapter title
====================================
[![DOI](https://zenodo.org/badge/DOI/YOUR_ZENODO_DOI.svg)](https://doi.org/YOUR_ZENODO_DOI)
![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![GitHub release](https://img.shields.io/github/v/release/YOUR_ORG/YOUR_REPO?logo=github)

## Contents

- [Contents](#contents)
- [Introduction](#introduction)
- [Repository structure](#respository-structure)
- [Key concepts](#key-concepts)
- [Controlled vocabulary](#controlled-vocabulary)
- [Figures](#figures)

# Introduction and Purpose

This is a template respository for the management and submission of IPCC AR7 figures. This repository is meant to store report figures at the chapter level, along with the data and code necessary to reproduce the figures. We acknowledge that publishing clean code and data is time-consuming, and that many figures don't survive the rounds of reviews, so we're only expecting code and data to be prepared for the Final Government Draft (FGD), not the First Order Draft (FOD) or Second Order Draft (SOD). However, we also know that delaying the data and code preparation process at the last minute will be painful for everyone involved because it will pile on the final publication rush. What we're proposing is a gradual approach to data and code curation, where each draft adds a bit more content to the repository for the sake of building experience and resolving issues in a stress-free environment.

# Repository structure
The repository structure is described below. You should create one repository for each chapter and for each draft.
* fig99_01: 
** data: The data/ folder is where you should store data to create the figure. It is meant to be self-contained, and include all information displayed in the figure. The data included here should require no substantial transformation to be used in the figure. This means for example that data units should match figure units.
** code: The code/ folder is where you should store the code used to analyse input data and create the data for the figure, if any. If no such code is necessary, simply remove this directory.
** figure: The figure/ folder is where you should upload the figure image file. 
* src: The src/ folder contains shared, reusable code used across multiple figures and analyses in this project. 
* env: The env/ folder contains environment specification files and documentation necessary to recreate the software environment used in this project. This ensures that analyses and figures can be reproduced reliably across different systems.

# Key concepts
– By *data*, we mean here the data displayed in the figure, not the source datasets they derive from. Please do not commit large input datasets in this repository;
– By *metadata*, we mean the information about the figure, such as its title, caption, authors, and references. This information is captured in a CITATION.cff file, documented here.

# Controlled vocabulary

Whenever a template includes fields for `<report>, <draft>, <chapter>` or `<figure>`, please use abbreviations from the table below.

| Type        | Full name                                 | Abbreviation |
|-------------|-------------------------------------------|-------------|
| ``report``  |                                           |             |  
|             | Special Report on Cities                  | src         |
|             | Working Group I                           | wg1         |
|             | Working Group II                          | wg2         |
|             | Working Group III                         | wg3         |
|             | Synthesis Report                          | syr         |
| ``draft``   |                                           |             |
|             | Zero Order Draft                          | zod         | 
|             | First Order Draft                         | fod         |
|             | Second Order Draft                        | sod         |
|             | Final Government Draft                    | fgd         |
| ``chapter`` |                                           |             |
|             | Summary for Policymakers                  | spm         |
|             | Technical Summary                         | ts          |
|             | Chapter 1                                 | ch1         |
|             | Cross-Chapter Paper 1                     | ccp1        |
|             | Annex III                                 | ann3        |
|             | Atlas                                     | atlas       |
| ``figure``  |                                           |             |
|             | Figure 4.1                                | fig1        |
|             | Cross-Chapter Box 4.1, Figure 1           | ccb1fig1  |
|             | Cross-Section Box TS.1, Figure 1          | csb1fig1  |
|             | Box 4.1, Figure 1                         | box1fig1  |
|             | Frequently Asked Questions 4.1, Figure 1  | faq1fig1  |

## Figures

For ease of reference and review by the TSU, please list all figures in this chapter, as indicated below.

Example:

| Figure Folder | Preview | Figure Title |
|---------------|---------|-------------|
| [fig99_01](./figures/fig99_01/) | <img src="./fig99_01/figure/ar6_wg1_chap3_figure3_4_surface_temp_anomaly.png" width="300"> | Title of fig99_01 |
| [fig99_02](./figures/fig99_02/) | link to figure | Title of fig99_02 |
|  |  |  |
|  |  |  |
|  |  |  |

