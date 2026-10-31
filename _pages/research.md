---
layout: page
title: research
permalink: /research/
description: Where my work is heading, and where you could join in.
nav: true
nav_order: 2
redirect_from:
  - /teaching/
---

Sound lets us monitor life continuously, non-invasively, and at scale, but only if we can turn hours of audio into something ecologists can trust. My work sits on three problems that stand between a microphone in the field and a reliable picture of biodiversity. Each section below describes where I'm heading, who I'm working with, and what's come out of it so far.

If one of these overlaps with what you want to work on, as a student, postdoc or collaborator, [get in touch](mailto:burooj.ghani@naturalis.nl).

[Soundscape analysis and discovery](#soundscape-analysis-and-discovery) · [Representation learning for bioacoustics](#representation-learning-for-bioacoustics) · [Automated species recognition](#automated-species-recognition)

---

## Soundscape analysis and discovery

Most of what a field recorder captures doesn't match any class in a trained model: species nobody labelled, calls we've never heard, and sounds that may not be biological at all. In the places where monitoring matters most, such as tropical forests, rivers and the sea, labelled data is scarce and the unknowns outnumber the knowns. A species classifier can't tell you what it hasn't been told to look for.

This is the direction I'm most excited about: moving from *recognising* sounds to *understanding* soundscapes. That means finding structure in unlabelled audio, flagging what's new, and deciding where a human expert's time is best spent. Methods I'm interested in include clustering and novelty detection in embedding space, open-set recognition, and active learning loops that build labelled data efficiently, starting from almost none.

**People**
- **Vincent Kather**, PhD candidate (co-supervised with [name]), is developing methods for detecting and characterising unknown sounds. He also built [bacpipe]([link]), [one-line description of bacpipe].
- [MSc/BSc students: name, thesis topic, year]

**Selected outputs**
- [Vincent's first paper: title, venue, link]
- [bacpipe]([link])

---

## Representation learning for bioacoustics

A good representation of animal sound does most of the heavy lifting. If embeddings capture what makes calls distinct, a classifier for a new species group can be built from a handful of examples, and unknown sounds can be explored without labels. My early work showed that embeddings learned from global birdsong transfer surprisingly well, even to taxa that aren't birds. Since then I've been asking when and why transfer works, how best to adapt large pretrained models to small, specialised datasets, and how far bioacoustic foundation models generalise beyond the data they were trained on.

{% include figure.html path="assets/img/tsne.jpg" class="img-fluid rounded z-depth-1" figure_class="figure-narrow" caption="Birdsong embeddings from [model], coloured by species: similar calls cluster together." %}

This area connects the other two: better representations make recognition cheaper and discovery possible.

**People**
- **Hilde Hummel**, PhD candidate (co-supervised with [name]), works on deep learning for underwater acoustics, including how well embeddings transfer to underwater sound.
- [MSc/BSc students: name, thesis topic, year]

**Selected outputs**
- [Global birdsong embeddings enable superior transfer learning for bioacoustic classification](https://www.nature.com/articles/s41598-023-49989-z). *Scientific Reports*, 2023.
- [Transfer learning methods, pretrained models and dataset characteristics in birdsong classification](https://www.nature.com/articles/s41598-025-00996-2) [replace with exact title]. *Scientific Reports*, 2025.
- [Hilde's papers, once out]
- Co-organiser, NeurIPS 2025 workshop on [AI for Non-Human Animal Communication](https://aiforanimalcomms.org).

---

## Automated species recognition

Species recognition is the workhorse of passive acoustic monitoring, and it's far from solved once you leave well-recorded birds. I build recognisers across taxa, including birds, bats, insects and frogs, each with its own challenges: ultrasonic calls, tiny datasets, closely related species that sound almost identical, and recordings that look nothing like the training data.

{% include figure.html path="assets/img/pipeline.jpg" class="img-fluid rounded z-depth-1" figure_class="figure-narrow" %}

Increasingly, my focus is on what happens *after* the model: making predictions reliable enough to support ecological conclusions. That includes calibration and per-species thresholds, honest evaluation on independent data, and using ecological knowledge, such as geography and taxonomy, to make models more useful rather than just more accurate.

**People**
- [Collaborators, e.g. Naturalis colleagues, with links]
- Welmoed Eversteijn, MSc thesis on deep learning for bats, 2026.
- Jagoda Hanuszewicz, MSc thesis on deep learning for anurans, 2026.
- Syed Aadam Ahmad, MSc thesis on bioacoustics and machine learning for avifauna monitoring in Kashmir, 2024.
- Sophie Van der Voorst and Linde Zandvliet, project on AI-based avian sound recognition in transect monitoring, 2024.

**Selected outputs**
- [AvesEcho](https://gitlab.com/arise-biodiversity/DSI/algorithms/avesecho-v1), a bird sound recogniser and the first ML model hosted on [Xeno-canto](https://xeno-canto.org/article/299).
- [ChiroEcho: [exact title]]([link]). CV4Ecology workshop, ECCV 2026. Recognition of European bats, using geographic priors to extend coverage beyond the trained species.
- [InsectSet459](https://arxiv.org/abs/2503.15074), a benchmark for insect sound classification.
- [Twelve quick tips for applying deep learning to animal sounds](https://journals.plos.org/ploscompbiol/article?id=10.1371%2Fjournal.pcbi.1014604). *PLOS Computational Biology*, 2026.

---

## Projects and funding

My work is funded through the [Horizon Europe](https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-europe_en) projects [MAMBO](https://mambo-project.eu), [GUARDEN](https://guarden.org) and [TETTRIs](https://www.ecsa.ngo/cases/tettris/), where I develop audio recognition algorithms for European taxa including birds, bats, marine mammals, pollinating insects and grasshoppers.

---

## Past students and mentoring

- 2026 - Supervising Welmoed Eversteijn and Jagoda Hanuszewicz on their masters thesis projects on deep learning for bats and anurans, respectively.
- 2025 - Supervising Hilde Hummel on her PhD titled “Machine learning algorithms for underwater acoustics”.
- 2024 - Supervising Vincent Kather on his PhD titled “Identifying unknown species and unknown sounds using machine learning”.
- 2024 - Supervised Sophie Van der Voorst and Linde Zandvliet on their project titled “AI-Based Avian Sound Recognition in Transect Monitoring”.
- 2024 - Supervised Syed Aadam Ahmad on his masters thesis titled "Integrating bioacoustics and machine learning for avifauna monitoring in Kashmir".
- 2023 - Supervised Drew Priebe ([Tilburg University](https://www.tilburguniversity.edu)) on his BSc thesis titled: “Efficient speech detection in environmental audio using acoustic recognition and model distillation”.
- 2023 - Supervised six students from [HvA Amsterdam](https://www.hva.nl) on their project on automated audio classification titled: [“Sing A Song”](https://vriesn23.dev.hihva.nl/aai-naturalis-1/) through [ARISE](https://www.arise-biodiversity.nl).

Please [contact me via email](mailto:burooj.ghani@naturalis.nl) for enquiries about BSc or MSc thesis projects at Naturalis Biodiversity Center.
