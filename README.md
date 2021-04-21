# APE-backtranslation
---
This repository is to distribute data that is introduced in the EACL 2021 paper
"[*Adaptation of Back-translation to Automatic Post-Editing for Synthetic Data Generation*](https://www.aclweb.org/anthology/2021.eacl-main.322)".   
You can download the data at http://kle.postech.ac.kr/data/ape/eacl21.

- [Introduction](#-introduction)
- [Files](#-files)
  - [escape.en](#escapeen)
  - [escape.de](#escapede)
  - [escape.bg.nmt](#escapebgnmt)
  - [escape.bg.pbsmt](#escapebgpbsmt)
  - [escape.fg.nmt](#escapefgnmt)
  - [escape.fg.pbsmt](#escapefgpbsmt)
- [References](#-references)

## Introduction
---
The data collection consists of
a source text file ([<span style="color:#ff0c93">escape.en</span>](#escapeen)),
a reference text file ([<span style="color:#ff0c93">escape.de</span>](#escapede)),
and **four different synthetic MT output text files**
([<span style="color:#ff0c93">escape.bg.nmt</span>](#escapebgnmt),
[<span style="color:#ff0c93">escape.bg.pbsmt</span>](#escapebgpbsmt),
[<span style="color:#ff0c93">escape.fg.nmt</span>](#escapefgnmt),
and [<span style="color:#ff0c93">escape.fg.pbsmt</span>](#escapefgpbsmt)).   
One same source text and reference text go for all of the four synthetic MT outputs, and both of them are the same as in [*eSCAPE*](https://www.aclweb.org/anthology/L18-1004/).  
We made the four synthetic MT output texts, two texts for each of two MT-system classes (NMT & PBSMT), by using two data-generation methods (Forward Generation, **FG**, & Backward Generation, **BG**) that we propose in our paper.   
All of the texts are tokenized by [*mosesdecoder*](https://github.com/moses-smt/mosesdecoder)'s tokenizer.   
Every line of each file is aligned with the same lines of the other files.   
Detailed explanation is given below.

## Files
---
---
### escape.en
This file contains source texts (*src*), each of which is an English sentence in principle.   
> <span style="font-family:Georgia">The aim of the invention is to produce hematopoietic cells that are suitable for active ingredient screening .</span>

### escape.de

This file contains reference texts (*ref*), each of which is a sound German sentence in principle.   
> <span style="font-family:Georgia">Der Erfindung liegt die Aufgabe zugrunde , hämatopoetische Zellen zu entwickeln , die für ein Wirkstoffscreening geeignet sind .</span>

---

### escape.bg.nmt

This file contains BG's synthetic MT outputs (*mt*<sub>BG</sub>) for the NMT class, each of which replaces eSCAPE's NMT text (*mt*).   
> <span style="font-family:Georgia">Der Erfindung liegt die Aufgabe zugrunde , hämatopoetische Zellen zu entwickeln , die für ein Wirkstoffscreening geeignet sind .</span>

### escape.bg.pbsmt

This file contains BG's synthetic MT outputs (*mt*<sub>BG</sub>) for the PBSMT class, each of which replaces eSCAPE's PBSMT text (*mt*).   
> <span style="font-family:Georgia">Der Erfindung liegt die Aufgabe zugrunde , hämatopoetische Zellen zu produzieren , die geeignet sind zur aktiven Bestandteil .</span>

### escape.fg.nmt

This file contains FG's synthetic MT outputs (*mt*<sub>FG</sub>) for the NMT class, each of which replaces eSCAPE's NMT text (*mt*).   
> <span style="font-family:Georgia">Aufgabe der Erfindung ist es , hämatopoetische Zellen herzustellen , die zur Wirkstoff-Screening geeignet sind .</span>

### escape.fg.pbsmt

This file contains FG's synthetic MT outputs (*mt*<sub>FG</sub>) for the PBSMT class, each of which replaces eSCAPE's PBSMT text (*mt*).   
> <span style="font-family:Georgia">Die Erfindung hat das Ziel , hämatopoetische Zellen zu produzieren , die sich zum Wirkstoffscreening eignen .</span>

## References
---
When you use our data for your work, please cite the following paper.   
## Adaptation of Back-translation to Automatic Post-Editing for Synthetic Data Generation   
WonKee Lee<sup>\*</sup>, Baikjin Jung<sup>\*</sup>, Jaehun Shin, Jong-Hyeok Lee.
[*Adaptation of Back-translation to Automatic Post-Editing for Synthetic Data Generation*](https://www.aclweb.org/anthology/2021.eacl-main.322)   
<span style="font-size:80%"><sup>\*</sup> Equal contribution.</span>

```bibtex
@inproceedings{lee-etal-2021-adaptation,
    title = "Adaptation of Back-translation to Automatic Post-Editing for Synthetic Data Generation",
    author = "Lee, WonKee  and
      Jung, Baikjin  and
      Shin, Jaehun  and
      Lee, Jong-Hyeok",
    booktitle = "Proceedings of the 16th Conference of the European Chapter of the Association for Computational Linguistics: Main Volume",
    month = apr,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2021.eacl-main.322",
    pages = "3685--3691"
}
```