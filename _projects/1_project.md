---
layout: page
title: Astronomical Transient Classification
description: BERT-based modeling of PLAsTiCC and ZTF light curves.
img: assets/img/10.jpg
importance: 1
category: work
related_publications: false
---

I build a transformer-based system that classifies astronomical transients using multi-band light curves from PLAsTiCC and ZTF. Time stamps are discretized, fluxes are log-scaled, and each object is transformed into a fixed-length tensor suitable for BERT encoders. The model incorporates contrastive supervision so that six photometric bands from the same source stay consistent, and conformal inference flags out-of-distribution events.

Key components:

- custom preprocessing pipelines for PLAsTiCC/ZTF data, including sparse time-series handling;
- transformer encoder that learns shared representations across passbands;
- fine-tuning head achieving ~75% accuracy on held-out validation data.

Source code and pretrained checkpoints are available on GitHub: [github.com/zhaoguanlan/PLASTICC](https://github.com/zhaoguanlan/PLASTICC).
