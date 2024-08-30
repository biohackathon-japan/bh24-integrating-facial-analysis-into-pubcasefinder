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

More than 6.2 \% of global population affected by rare diseases. Diagnosing patients with rare diseases is challenging because of the rarity and diversity of the disorders. It is often referred to as the "diagnostic odyssey" due to the long and complicated process of reaching a diagnosis. The facial analysis tools such as GestaltMatcher (GM)  [@citation:Hsieh2022-lw; @citation:Lesmann2024-wz] and Face2Gene [@citation:Gurovich2019-if; citation:Mishima2019-fm] have been developed to assist the diagnosis of rare diseases.
Although the whole exome sequencing technology is widely used for the diagnosis of rare disease, interpreting the huge number of variants is still a challenging task. 
Therefore, considering the clinical phenotypic information together with exome data is crucial.

The next-generation phenotyping approach to analyze the clinical information such as Human Phenotype Ontology (HPO) [@citation:Gargano2024-og] and facial image have been employed in many studies to assist the diagnosis of rare disorders.
PubCaseFinder [@citation:Fujiwara2018-ve; @citation:Yamaguchi2021-kg; @citation:Fujiwara2022-uc]
 is a tool that can search similar clinical cases from the literature and is widely used in rare disease diagnosis, especially in the Japanese society.
GestaltMatcher is the state-of-the-art deep facial phenotyping approach that trained on GestaltMatcher Database (GMDB), a largest facial image database for rare diseases compliant with FAIR principles.
In this study, we aim to integrate the facial image analysis, GestaltMatcher into PubCaseFinder to analyze the Japanese cohort.

We first benchmarked the performance of GestaltMatcher and PubCaseFinder on the GMDB dataset. Moreover, we focused on the Japanese patients. We collected the clinical information encoded to HPO terms and the facial image from the publcations in the [J-STAGE](https://www.jstage.jst.go.jp/) database. 

The diagnosis of rare diseases is challenging due to the rarity of the diseases and the lack of expertise. The facial analysis tools such as GestaltMatcher (GM) and Face2Gene have been developed to assist the diagnosis of rare diseases. The PubCaseFinder is a tool that can search similar clinical cases from the literature. The integration of facial analysis tools into PubCaseFinder can help the clinicians to diagnose the rare diseases more efficiently.

# Materials and Methods

## Data Source
The J-STAGE is a a public platform for scholarly publications in Japan. The site is developed and managed by the Japan Science and Technology Agency. Most of archived documents were written in Japanse. PDF files of peer-reviewed  clinical case reports in J-STAGE were searched manually using relevant words related to each syndrome, and downloaded manually.

## HPO term assignment
HPO terms were assined to each case repots by automatically and/or manually. Automatic HPO assignment was performed by using the free-text HPO term extraction function of PubCaseFinder

# Results
## Benchmarking on GMDB dataset

...

## Benchmarking on J-STAGE dataset
Table: Cases analyzed in this study. m: month, y: year.
| syndrome          | omim ID | age | sex  | deidentification | HPO term | DOI                    |
| --------          | ------  | --- | ---  | ---------------- | -------- | ---------------------- |
| Angelman Syndrome	| 105830	| 18m |	male | circles          |	+        | 10.11411/jspd.52.4_559 |

<!--
Cockayne syndrome	216400	4	female	Eyes are hidden.	https://doi.org/10.11251/ojjscn1969.10.465
Cockayne syndrome	216400	2	female	Eyes are hidden.	https://doi.org/10.11251/ojjscn1969.10.465
Cockayne syndrome	216400	12	male	Eyes are hidden.	https://doi.org/10.5794/jjoms.32.2274
Coffin-Lowry syndrome	303600	16	female	Eyes are hiddeen by small circles.	https://doi.org/10.11277/stomatology1952.46.177
Coffin-Lowry syndrome	303600	28	male	Eyes are hiddeen by small circles.	https://doi.org/10.14958/jjsdh.38.192
Coffin-Lowry syndrome	303600	46	male	Eyes are hiddeen by small circles.	https://doi.org/10.14958/jjsdh.38.192
Cornelia de Lange Syndrome	122470	4	female	Eyes are hidden	https://doi.org/10.11411/jspd1963.22.4_889
Cornelia de Lange Syndrome	122470	8 months	female	Whole face is shown. 	https://doi.org/10.11164/jjsps.25.7_1103
Kabuki syndrome	147920	5	female	Eyes are hidden.	https://doi.org/10.11411/jspd1963.31.1_121
Kabuki syndrome	147920	18	female	Eyes are shown. Black bar on the mouse.	https://doi.org/10.5631/jibirinsuppl1986.1989.Supplement32_169
Kabuki syndrome	147920	5	male	Eyes are hidden.	https://doi.org/10.5794/jjoms.42.729
Kabuki syndrome	147920	6 days	male	Eyes are hidden.	https://doi.org/10.5794/jjoms.37.795
Kabuki syndrome	147920	1	male	Eyes are hidden. Photo quality is low.	https://doi.org/10.5794/jjoms.37.795
Kabuki syndrome	147920	9	male	Eyes are hidden.	https://doi.org/10.11411/jspd1963.34.1_269
Kabuki syndrome	147920	5	male	Only upper face is shown	https://doi.org/10.5631/jibirin.85.1427
Kabuki syndrome	147920	7 months	male	Only upper face is shown	https://doi.org/10.5631/jibirin.85.1427
Kabuki syndrome	147920	4	female	Face is hidden by a bar	https://doi.org/10.11265/poms1991.8.2_39
Mucopolysaccharidosis I	607014	46	male	Face is hidden by a bar	https://doi.org/10.11281/shinzo1969.26.12_1220
Mucopolysaccharidosis II	607014	8	male	Face is hidden by a bar	https://doi.org/10.11411/jspd.54.4_507
Mucopolysaccharidosis II	607014	6	male	Face is hidden by a bar	https://doi.org/10.11289/otoljpn1974.13.468
Noonan Syndrome	163950	8 months	male	Whole face is shown. A paper in English.	https://doi.org/10.14930/jsma1939.40.75
Noonan Syndrome	163950	8	male	Whole face is shown. A paper in English.	https://doi.org/10.14930/jsma1939.40.75
Noonan Syndrome	163950	33	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1989.83.1902
Noonan Syndrome	163950	8	male	Face is hidden by a bar	https://doi.org/10.2334/josnusd.45.117
Noonan Syndrome	163950	3	male	Face is hidden by a bar	https://doi.org/10.5794/jjoms.42.929
Noonan Syndrome	163950	3	male	Face is hidden by a bar	https://doi.org/10.14958/jjsdh.36.118
Noonan Syndrome	163950	13	male	Face is hidden by a bar	https://doi.org/10.14958/jjsdh.36.118
Noonan Syndrome	163950	9	male	Face is hidden by a bar	https://doi.org/10.5794/jjoms.27.1056
Noonan Syndrome	163950	3	female	Face is hidden by circles	https://doi.org/10.14958/jjsdh.41.318
Prader-Willi Syndrome	176270	25	female	Face is hidden by a bar	https://doi.org/10.11340/skinresearch1959.41.58
Prader-Willi Syndrome	176270	6	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1928.67.7_548
Prader-Willi Syndrome	176270	7	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1928.67.7_548
Prader-Willi Syndrome	176270	10	female	Face is hidden by a bar	https://doi.org/10.11411/jspd1963.27.3_700
Prader-Willi Syndrome	176270	16	male	Face is hidden by a bar	https://doi.org/10.11340/skinresearch1959.31.402
Prader-Willi Syndrome	176270	25	male	Face is hidden by circles	https://doi.org/10.11255/jjmcp1992.15.19
Prader-Willi Syndrome	176270	15	female	Face is hidden by circles	https://doi.org/10.11277/stomatology1952.43.672
Prader-Willi Syndrome	176270	7	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1928.71.9_999
Prader-Willi Syndrome	176270	5	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1928.71.9_999
Prader-Willi Syndrome	176270	3	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1928.71.9_999
Prader-Willi Syndrome	176270	5	male	Face is hidden by a bar	https://doi.org/10.5980/jpnjurol1928.71.9_999
Prader-Willi Syndrome	176270	5	male	Face is hidden by a bar	https://doi.org/10.5794/jjoms.31.1513
Prader-Willi Syndrome	176270	4	male	Face is hidden by a bar	https://doi.org/10.11411/jspd1963.18.2_377
Rubinstein-Taybi Syndrome	180849	6	female	Whole face is shown.	https://doi.org/10.5035/nishiseisai.35.697
Rubinstein-Taybi Syndrome	180849	4	male	Mouth is hidden.	https://doi.org/10.4263/jorthoptic.29.239
Sotos syndrome	117550	10	male	Eyes are hidden.	https://doi.org/10.11411/jspd1963.34.5_1294
Sotos syndrome	117550	28	female	Eyes are hiddeen by small circles. Color.	https://doi.org/10.5794/jjoms.69.22
Williams-Beuen syndrome 	194050	41	female	Whole face is shown. A paper in English.	https://doi.org/10.1536/ihj.34.653
Williams-Beuen syndrome 	194050	10	female	Eyes are hidden.	https://doi.org/10.14958/jjsdh.43.129
Williams-Beuen syndrome 	194050	4	male	Face is hidden by circles	https://doi.org/10.11411/jspd.50.3_256
Williams-Beuen syndrome 	194050	23	male	Face is hidden by circles	https://doi.org/10.11411/jspd.50.3_256
Williams-Beuen syndrome 	194050	4	male	Face is hidden by short bars	https://doi.org/10.11411/jspd1963.41.5_912
Williams-Beuen syndrome 	194050	10	female	Face is hidden by a bar	https://doi.org/10.14958/jjsdh.43.129
Williams-Beuen syndrome 	194050	9	female	Face is hidden by circles	https://doi.org/10.14958/jjsdh.42.271
Williams-Beuen syndrome 	194050	10	male	Face is hidden by a bar	https://doi.org/10.5794/jjoms.34.1982
Williams-Beuen syndrome 	194050	41	female	Whole face is shown. 	https://doi.org/10.1536/ihj.34.653![image](https://github.com/user-attachments/assets/949c2d2d-c589-449f-8990-f7966dab75d5)
-->

# Discussion

...

## Acknowledgements

...

## References
<!-- 
References will be automatically added when we submit to BioHackrXiv. Instruction for authors below is commented out in the source.

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
