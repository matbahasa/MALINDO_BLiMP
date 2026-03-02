# MALINDO BLiMP (Malay/Indonesian Benchmark of Linguistic Minimal Pairs)

## Introduction
MALINDO BLiMP is a dataset for targeted syntactic evaluations of language models in Malay (zsm) and Indonesian (ind).  In building MALINDO BLiMP, we closely followed the procedure adopted by the developers of [JBLiMP (Japanese Benchmark of Linguistic Minimal Pairs)](https://github.com/osekilab/JBLiMP).  We collected our data from linguistics journals and books and created minimal pairs.  These minimal pairs are classified into 12 phenomena consisting of 45 paradigms.

MALINDO BLiMP is still under construction, so we are releasing a small part of it first before releasing the full version.

MALINDO BLiMP is licensed under a [Creative Commons Attribution 4.0 International (CC BY 4.0) license](https://creativecommons.org/licenses/by/4.0/).

## How to Cite
Nomoto, Hiroki, Sri Budi Lestari, David Moeljadi, Farhan Athirah binti Abdul Razak, Kazuya Inagaki and Masashi Furihata. 2026. [Challenges in building a benchmark of linguistic minimal pairs for low resource languages: The case of Malay and Indonesian](https://www.anlp.jp/proceedings/annual_meeting/2026/pdf_dir/Q1-6.pdf). <i>Proceedings of the Thirty-Second Annual Meeting of the Association for Natural Language Processing</i>, 381-386.

```bib
@InProceedings{NomotoEtAl26,
    author = {Nomoto, Hiroki and Lestari, Sri Budi and Moeljadi, David and Farhan Athirah binti Abdul Razak and Inagaki, Kazuya and Furihata, Masashi},
    year = {2026},
    title = {Challenges in building a benchmark of linguistic minimal pairs for low resource languages: The case of Malay and Indonesian},
    booktitle = {Proceedings of the Thirty-Second Annual Meeting of the {A}ssociation for {N}atural {L}anguage {P}rocessing},
    pages = {381-386},
    url = {https://www.anlp.jp/proceedings/annual_meeting/2026/pdf_dir/Q1-6.pdf}
}
```

## Contents
- `core/raw/`: Minimal pairs used for human validation (300 pairs for both Malay and Indonesian)
- `core/validated/`: Minimal pairs after human validation (174 pairs for Malay and 189 pairs for Indonesian)
- `core/validation/`: Results of human validation (acceptability judgement experiment)

## Data Format
|Name|Description|
|----|-----------|
|ID | ID of the minimal pair|
|original\_language| Language of the original sentence|
|{good/bad}\_diacritic| Acceptability judgement in the source (`g` = no diacritic)|
|{good/bad}\_sentence\_raw| Raw sentence in the source (not necessarily in the target language)|
|{good/bad}\_sentence| MALINDO BLiMP sentence (translated if the raw sentence is not in the target language)|
|{good/bad}\_translation| English translation|
|{good/bad}\_source| Author and publication year of the source|
|{good/bad}\_page| Page number where the relevant sentence appears in the source|
|{good/bad}\_num| Example number of the relevant sentence in the source|
|phenomenon| Categorization based on linguistic phenomenon|
|paradigm| Sub-categorization of phenomenon|
