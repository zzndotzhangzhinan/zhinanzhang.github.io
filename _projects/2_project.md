---
layout: page
title: WeChat Article Readership Prediction
description: Text + metadata model to forecast article views.
img: assets/img/8.jpg
importance: 2
category: work
giscus_comments: false
---

This project predicts the readership of WeChat public-account articles. Each article is encoded with a transformer-based text encoder plus engineered metadata features (publish time, category, follower baseline). A gradient boosting layer produces calibrated view-count forecasts so that editors know which stories resonate with readers.

Highlights:

- cleaned millions of historical articles and normalized view statistics to reduce platform policy shifts;
- combined Chinese-language pretrained encoders with lightweight attention pooling to stay efficient;
- delivered actionable dashboards for editors to compare predicted and actual traffic in real time.

Implementation details and experiments can be found on GitHub: [github.com/zhaoguanlan/WeChat_TextClassifier](https://github.com/zhaoguanlan/WeChat_TextClassifier).
