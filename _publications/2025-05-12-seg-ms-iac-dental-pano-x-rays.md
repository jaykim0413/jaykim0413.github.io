---
title: "Generalized Segmentation for Maxillary Sinus and Mandibular Canal in Dental Panoramic X-rays"
collection: publications
category: conferences
# permalink: /publications/2025-05-12-seg-ms-iac-dental-pano-x-rays
excerpt: 'In this study, we aimed to enhance the accuracy of dental treatments, such as implant insertions, by employing deep learning to precisely identify and delineate the maxillary sinus and mandibular canal in panoramic dental X-rays. To achieve this, we constructed a labeled panoramic dental X-ray dataset. Utilizing this dataset, we proposed an optimal model by integrating UNet with a Convolutional Block Attention Module (CBAM) for segmentation tasks. CBAM effectively reduced false positives through attention mechanisms, improving the model’s precision. Additionally, to evaluate the model’s performance across various environments, we performed external validation using an open dataset. To further improve external validation performance, we introduced a novel augmentation technique by modifying CutMix to suit our specific task requirements. The modified CutMix reduced false negatives by leveraging shape bias, enhancing the model’s sensitivity. Our experiments demonstrated that the developed model achieved not only the highest test performance within the constructed dataset, but also robust generalization performance on external validation. This indicates the generalizability of our model across diverse clinical settings.'
date: 2025-05-12
venue: 'BioImage Computing Workshop, European Conference on Computer Vision 2024 (BIC ECCV 2024)'
paperurl: 'https://rdcu.be/exo7Q'
citation: '*Kim, J.W., Bae, S. (2025). Generalized Segmentation for Maxillary Sinus and Mandibular Canal in Panoramic X-Rays. In: Del Bue, A., Canton, C., Pont-Tuset, J., Tommasi, T. (eds) Computer Vision – ECCV 2024 Workshops. ECCV 2024. Lecture Notes in Computer Science, vol 15638. Springer, Cham. https://doi.org/10.1007/978-3-031-91721-9_17*'
---

## Overview

Panoramic dental X-rays are the standard first look before procedures like
implant placement, but two of the structures that matter most for surgical
planning — the **maxillary sinus** and the **mandibular canal** — are hard to
delineate reliably. This work builds a deep-learning segmentation model that
identifies both well enough to generalize across different clinical sources.

## Approach

- **Dataset.** We constructed a labeled panoramic dental X-ray dataset for the
  two target structures.
- **Model.** A **U-Net** backbone with a **Convolutional Block Attention Module
  (CBAM)**. The attention mechanism suppressed false positives by focusing the
  network on the relevant anatomy, improving precision.
- **Generalization.** To test robustness beyond our own data, we ran **external
  validation on an open dataset**, then introduced a **modified CutMix**
  augmentation tailored to this task. By leveraging shape bias it reduced false
  negatives and raised sensitivity — the augmentation and regularization
  strategy expanded the effective training data roughly **1200×**.

## Results

The model reached the best test performance on our constructed dataset while
also holding up under external validation — evidence it generalizes across
clinical settings rather than overfitting to one source.

<!-- TODO: add headline numbers (e.g. Dice / IoU, internal vs. external) if
     you'd like quantitative results shown here. -->

## Links

- **Code:** [github.com/jaykim0413/seg-pano-extended](https://github.com/jaykim0413/seg-pano-extended)
- **DOI:** [10.1007/978-3-031-91721-9_17](https://doi.org/10.1007/978-3-031-91721-9_17)
- Presented at the **BioImage Computing Workshop, ECCV 2024**.
