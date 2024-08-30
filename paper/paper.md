---
title: 'BioHackathon2024 report: Integrating Facial Analysis into PubCaseFinder'
title_short: 'BH24: GestaltMatcher and PubCaseFinder'
tags:
  - rare diseases
  - human genetics
  - HPO
  - diagnosis assistance
authors:
  - name: Tzung-Chen Hsieh
    affiliation: 1
  - name: Toyofumi Fujiwara
    affiliation: 2
  - name: Hiroyuki Mishima
    orcid: 0000-0001-5050-2509
    affiliation: 3
affiliations:
  - name: Institute for Genomic Statistics and Bioinformatics, University Hospital Bonn, Rheinische Friedrich-Wilhelms-Universität Bonn, Bonn, Germany
    index: 1
  - name: Second Affiliation
    index: 2
  - name: Department of Human Genetics, Atomic Bomb Disease Institute, Nagasaki University, Nagasaki, Japan
    index: 3
date: 30 November 2024
cito-bibliography: paper.bib
event: BH24
biohackathon_name: "BioHackathon 2024"
biohackathon_url:   "https://2024.biohackathon.org/"
biohackathon_location: "Fukushima, Japan, 2024"
group: GestaltMacher-PubCaseFinder group
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/biohackathon-japan/bh24-integrating-facial-analysis-into-pubcasefinder

# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Tzung-Chen Hsieh \emph{et al.}
---

# Introduction

More than 6.2 \% of global population affected by rare diseases. Diagnosing patients with rare diseases is challenging because of the rarity and diversity of the disorders. It is often referred to as the "diagnostic odyssey" due to the long and complicated process of reaching a diagnosis. The facial analysis tools such as GestaltMatcher (GM) and Face2Gene have been developed to assist the diagnosis of rare diseases.
Although the whole exome sequencing technology is widely used for the diagnosis of rare disease, interpreting the huge number of variants is still a challenging task. 
Therefore, considering the clinical phenotypic information together with exome data is crucial.

The next-generation phenotyping approach to analyze the clinical information such as Human Phenotype Ontology (HPO) and facial image have been employed in many studies to assist the diagnosis of rare disorders.
PubCaseFinder is a tool that can search similar clinical cases from the literature and is widely used in rare disease diagnosis, especially in the Japanese society.
GestaltMatcher is the state-of-the-art deep facial phenotyping approach that trained on GestaltMatcher Database (GMDB), a largest facial image database for rare diseases compliant with FAIR principles.
In this study, we aim to integrate the facial image analysis, GestaltMatcher into PubCaseFinder to analyze the Japanese cohort.

We first benchmarked the performance of GestaltMatcher and PubCaseFinder on the GMDB dataset. Moreover, we focused on the Japanese patients. We collected the clinical information encoded to HPO terms and the facial image from the publcations in J-Stage database. 


The diagnosis of rare diseases is challenging due to the rarity of the diseases and the lack of expertise. The facial analysis tools such as GestaltMatcher (GM) and Face2Gene have been developed to assist the diagnosis of rare diseases. The PubCaseFinder is a tool that can search similar clinical cases from the literature. The integration of facial analysis tools into PubCaseFinder can help the clinicians to diagnose the rare diseases more efficiently.

As part of the BioHackathon 2024, we here report...

GestaltMacher [@citation:Hsieh2022-lw]

GestaltMatcher Databaase [@citation:Lesmann2024-wz]

PubCaseFinder [@citation:Fujiwara2018-ve; @citation:Yamaguchi2021-kg; @citation:Fujiwara2022-uc]

Limitations of Face2Gene in Japanese population [@citation:Mishima2019-fm]

Human Phenotype Ontology (HPO) [@citation:Gargano2024-og]

# Materials and Methods

## Data Source
The [J-STAGE](https://www.jstage.jst.go.jp/) is a a public platform for scholarly publications in Japan. The site is developed and managed by the Japan Science and Technology Agency. Each PDF files of peer-reviewed and published clinical case report in J-STAGE is downloaded.

## HPO term assignment
HPO terms were assined to each case repots by automatically and/or manually. Automatic HPO assignment was performed by using the free-text HPO term extraction function of PubCaseFinder


# Results
## Benchmarking on GMDB dataset

## Benchmarking on J-STAGE dataset



# Discussion

...

## Acknowledgements

...

## References
References will be automatically added when we submit to BioHackrXiv. Instruction for authors below is commented out in the source.


<!-- 
# Formatting

This document use Markdown and you can look at [this tutorial](https://www.markdowntutorial.com/).

## Subsection level 2

Please keep sections to a maximum of only two levels.

## Tables and figures

Tables can be added in the following way, though alternatives are possible:

Table: Note that table caption is automatically numbered and should be
given before the table itself.

| Header 1 | Header 2 |
| -------- | -------- |
| item 1 | item 2 |
| item 3 | item 4 |

A figure is added with:

![Caption for BioHackrXiv logo figure](./biohackrxiv.png)

# Other main section on your manuscript level 1

Lists can be added with:

1. Item 1
2. Item 2

# Citation Typing Ontology annotation

You can use [CiTO](http://purl.org/spar/cito/2018-02-12) annotations, as explained in [this BioHackathon Europe 2021 write up](https://raw.githubusercontent.com/biohackrxiv/bhxiv-metadata/main/doc/elixir_biohackathon2021/paper.md) and [this CiTO Pilot](https://www.biomedcentral.com/collections/cito).
Using this template, you can cite an article and indicate _why_ you cite that article, for instance DisGeNET-RDF [@citesAsAuthority:Queralt2016].

The syntax in Markdown is as follows: a single intention annotation looks like
`[@usesMethodIn:Krewinkel2017]`; two or more intentions are separated
with colons, like `[@extends:discusses:Nielsen2017Scholia]`. When you cite two
different articles, you use this syntax: `[@citesAsDataSource:Ammar2022ETL; @citesAsDataSource:Arend2022BioHackEU22]`.

Possible CiTO typing annotation include:

* citesAsDataSource: when you point the reader to a source of data which may explain a claim
* usesDataFrom: when you reuse somehow (and elaborate on) the data in the cited entity
* usesMethodIn
* citesAsAuthority
* citesAsEvidence
* citesAsPotentialSolution
* citesAsRecommendedReading
* citesAsRelated
* citesAsSourceDocument
* citesForInformation
* confirms
* documents
* providesDataFor
* obtainsSupportFrom
* discusses
* extends
* agreesWith
* disagreesWith
* updates
* citati
-->
