---
layout: page
title: research
permalink: /research/
description: 
nav: true
nav_order: 1
redirect_from:
  - /teaching/
---

Passive acoustic monitoring makes it possible to observe animal communities continuously, non-invasively and at large spatial scales. Its value for ecology, however, depends on our ability to convert large volumes of field recordings into information reliable enough to support ecological inference. My research addresses three interrelated problems that lie between data collection in the field and robust estimates of biodiversity. A broader perspective on the field is given in [Twelve quick tips for applying deep learning to animal sounds](https://journals.plos.org/ploscompbiol/article?id=10.1371%2Fjournal.pcbi.1014604).

{% include figure.html path="assets/img/journal.pcbi.1014604.g001.PNG" class="img-fluid rounded z-depth-1" figure_class="figure-narrow" caption=" An integrated lifecycle for bioacoustic machine learning." %}

The sections below outline each research theme, the people involved, and the main outputs to date.

Students, researchers and collaborators with interests in any of these areas are welcome to [get in touch](mailto:burooj.ghani@naturalis.nl).

[Representation learning for bioacoustics](#representation-learning-for-bioacoustics) · [Automated species recognition](#automated-species-recognition) · [Soundscape analysis and discovery](#soundscape-analysis-and-discovery) 

---

## Representation learning for bioacoustics

Learned representations are central to computational bioacoustics. Embeddings that capture the acoustic features distinguishing one vocalisation from another allow classifiers for new taxa to be trained from few labelled examples, and make it possible to explore unlabelled recordings. In earlier work, we showed that embeddings learned from large-scale birdsong data transfer effectively to other bioacoustic classification tasks, including taxa other than birds. My current work examines the conditions under which such transfer succeeds, strategies for adapting large pretrained models to small, specialised datasets, and the extent to which bioacoustic foundation models generalise beyond their training distribution.

{% include figure.html path="assets/img/tsne.jpg" class="img-fluid rounded z-depth-1" figure_class="figure-narrow" caption="Animal sound embeddings: similar sounds cluster together." %}

Advances in representation learning underpin the other two themes: more informative embeddings reduce the annotation effort required for species recognition and enable the discovery of unknown sound sources.

**People**
- **Hilde Hummel**, PhD candidate, works on deep learning for underwater acoustics, including the transferability of pretrained embeddings to underwater sound.

**Selected outputs**
- [Global birdsong embeddings enable superior transfer learning for bioacoustic classification](https://www.nature.com/articles/s41598-023-49989-z). *Scientific Reports*, 2023.
- [Transfer learning methods, pretrained models and dataset characteristics in birdsong classification](https://www.nature.com/articles/s41598-025-00996-2) [replace with exact title]. *Scientific Reports*, 2025.
- [Linear probing enables Ship-Radiated Noise recognition with pretrained audio embeddings](https://www.sciencedirect.com/science/article/pii/S1574954126001159) *Ecological Informatics*, 2026 
- Co-organiser, NeurIPS 2025 workshop on [AI for Non-Human Animal Communication](https://aiforanimalcomms.org).

---

## Automated species recognition

Automated species recognition is a core component of passive acoustic monitoring, yet it remains a challenging problem beyond well-documented species. We have developed classifiers for a range of taxa, including birds, bats, insects and anurans, each of which poses distinct challenges: ultrasonic vocalisations, limited training data, acoustically similar closely related species, and pronounced domain shift between training data and field recordings.

{% include figure.html path="assets/img/pipeline.jpg" class="img-fluid rounded z-depth-1" figure_class="figure-narrow" %}

An increasing focus of my work is the reliability of model outputs for ecological inference. This includes calibration and species-specific decision thresholds, rigorous evaluation on independent test data, and the integration of ecological prior knowledge, such as geographic range and taxonomic structure, so that model predictions are judged by their ecological utility rather than by accuracy alone.

**People**
- **Welmoed Eversteijn**, MSc thesis on deep learning for bats, 2026.
- **Jagoda Hanuszewicz**, MSc thesis on deep learning for anurans, 2026.

**Selected outputs**
- [AvesEcho](https://gitlab.com/arise-biodiversity/DSI/algorithms/avesecho-v1), a bird sound classifier and the first machine learning model hosted on [Xeno-canto](https://xeno-canto.org/article/299).
- [ChiroEcho: extending automated bat vocalisation classification beyond the learned taxonomy](https://arxiv.org/pdf/2608.18191). Classification of European bat species, using geographic priors to extend coverage beyond the species seen during training. *CV4Ecology workshop, ECCV 2026.*
- [A dataset of insect sounds from 459 species for bioacoustic machine learning](https://www.nature.com/articles/s41597-026-07123-4), a benchmark for insect sound classification. *Scientific Data*, 2025.

---

## Soundscape analysis and discovery

A large proportion of the sounds captured in field recordings do not correspond to any class known to a trained model: unlabelled species, undescribed call types, and sounds of non-biological origin. In the ecosystems where monitoring is most needed, such as tropical forests, freshwater systems and the marine environment, labelled data are scarce and unknown sound sources often outnumber known ones. Closed-set classifiers, by design, cannot identify sounds outside their training classes.

Our work in this area therefore shifts the emphasis from the *recognition* of individual sounds to the *characterisation* of soundscapes. This involves identifying structure in unlabelled audio, detecting novel sound sources, and prioritising the recordings that most warrant expert annotation. Methods of interest include clustering and novelty detection in embedding space, open-set recognition, and active learning approaches for building labelled datasets efficiently from very limited initial annotation.

**People**
- **Vincent Kather**, PhD candidate, develops methods for detecting and characterising unknown sounds. He also developed [bacpipe](https://github.com/bioacoustic-ai/bacpipe), a Python package that makes bioacoustic deep learning models more accessible.
- **Anielkoemar Gangadin**, PhD candidate, studies the diversity, acoustic ecology, and biogeography of cicadas in Suriname.


**Selected outputs**
- [Clustering and novel class recognition: evaluating bioacoustic deep learning feature extractors](https://arxiv.org/pdf/2504.06710)
- [Bacpipe: A Python package to make bioacoustic deep learning models accessible](https://besjournals.onlinelibrary.wiley.com/doi/full/10.1111/2041-210x.70406)

---


## Projects and funding

A lot of above research is funded by the [Horizon Europe](https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en) projects [MAMBO](https://mambo-project.eu), [GUARDEN](https://guarden.org) and [TETTRIs](https://www.ecsa.ngo/cases/tettris/).

---

## Past students

- 2024 - Supervised Sophie Van der Voorst and Linde Zandvliet on their project titled “AI-Based Avian Sound Recognition in Transect Monitoring”.
- 2024 - Supervised Syed Aadam Ahmad on his masters thesis titled "Integrating bioacoustics and machine learning for avifauna monitoring in Kashmir".
- 2023 - Supervised Drew Priebe ([Tilburg University](https://www.tilburguniversity.edu)) on his BSc thesis titled: “Efficient speech detection in environmental audio using acoustic recognition and model distillation”.
- 2023 - Supervised six students from [HvA Amsterdam](https://www.hva.nl) on their project on automated audio classification titled: [“Sing A Song”](https://vriesn23.dev.hihva.nl/aai-naturalis-1/) through [ARISE](https://www.arise-biodiversity.nl).

Prospective BSc and MSc students interested in thesis projects at Naturalis Biodiversity Center are welcome to [contact me by email](mailto:burooj.ghani@naturalis.nl).
