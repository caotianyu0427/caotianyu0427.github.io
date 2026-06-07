---
title: "JuncForge"
summary: "qPCR primer design pipeline for cryptic exon (CE) junction detection in mouse genomes."
date: 2025-06-01
tags:
  - Bioinformatics
  - RNA Splicing
  - qPCR
links:
  - icon: brands/github
    url: https://github.com/caotianyu0427/JuncForge
    label: Code
image:
  focal_point: Smart
---

## Overview

JuncForge is a computational pipeline for designing qPCR primer pairs that span cryptic exon (CE) splice junctions. It targets applications in RNA splicing research, including studies of TDP-43 loss of function and cryptic exon inclusion in neurodegeneration.

## What it does

Given GenBank files annotating a cryptic exon within an intron, the pipeline:

1. Locates CE features and their left/right junctions
2. Designs primer pairs via Primer3 with junction-spanning constraints
3. Filters candidates with pair-wise BLAST against genome and curated RefSeq mRNA
4. Retains only primers expected to amplify the CE-containing transcript

## Tech stack

Python, Primer3, BLAST

## Links

- GitHub: https://github.com/caotianyu0427/JuncForge
