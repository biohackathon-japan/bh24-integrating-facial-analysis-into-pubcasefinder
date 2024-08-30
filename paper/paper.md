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
  - name: First Affiliation
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

As part of the BioHackathon 2024, we here report...

GestaltMacher [@citation:Hsieh2022-lw]

GestaltMatcher Databaase [@citation:Lesmann2024-wz]

PubCaseFinder [@citation:Fujiwara2018-ve; @citation:Fujiwara2022-uc]

Limitations of Face2Gene in Japanese population [@citation:Mishima2019-fm]

# Materials and Methods

## Data Source
The [J-STAGE](https://www.jstage.jst.go.jp/) is a a public platform for scholarly publications in Japan. The site is developed and managed by the Japan Science and Technology Agency. Each clinical case report in J-STAGE is downloaded. 


maintained by .

# Results

# Discussion

...

## Acknowledgements

...

## References


---

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
* citation: generic citation


# Results


# Discussion

...

## Acknowledgements

...

## References
