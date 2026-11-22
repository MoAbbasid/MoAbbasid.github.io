---
layout: page
permalink: /projects/index.html
title: Projects
---

# Projects

{% include click-gif-assets.html %}

## Malaysia Seat Analytics

{% include click-gif.html video="/assets/malaysia-seat-analytics-demo.mp4" poster="/assets/malaysia-seat-analytics-poster.jpg" alt="Walkthrough of the Malaysia Seat Analytics dashboard" w="880" h="519" %}

Streamlit dashboard joining open socio-economic data with GE-14 and GE-15 election results across all 222 Malaysian parliamentary constituencies.

**Stack:** Python, pandas, Plotly, Streamlit. Open data from DOSM and ElectionData.MY.

**Highlights: what the data shows**

* The median seat has a median household income of RM 5,350 a month. Seat medians range from RM 2,851 (Kota Marudu, Sabah) to RM 15,867 (Segambut, Kuala Lumpur).
* 117 of 222 seats (52.7%) changed winning coalition between GE-14 and GE-15.
* Income and poverty are strongly negatively correlated at seat level (r = -0.64).

**Code available on request.**

## RoadWork Cone Mapping

{% include click-gif.html video="/assets/roadwork-cone-mapping-demo.mp4" poster="/assets/roadwork-cone-mapping-poster.jpg" alt="Walkthrough of RoadWork Cone Mapping: detected cones with relative gaps, then a Los Angeles route map" w="720" h="422" %}

Cone detection on dashcam frames from the CMU ROADWork dataset, with relative gaps between neighbouring cones and a GPS route map of cone counts along a Los Angeles street.

**Stack:** Python, Ultralytics YOLO26, OpenCV, Folium. Data: CMU ROADWork (ODC-Attribution).

**Highlights: results**

* YOLO26s fine-tuned for 50 epochs reaches mAP50 0.747 (precision 0.804, recall 0.717) on the 5,396 cone instances in the validation set.
* Gaps between neighbouring cones are scaled from cone height, assuming a 28 in cone, so they are relative rather than calibrated distances.
* On a 30-frame stretch of Los Angeles, 63 cones were detected and mapped in capture order along the GPS route.

**Details:** [Interactive route maps](/projects/roadwork-cone-mapping/)

**Code:** [github.com/MoAbbasid/roadwork-cone-mapping](https://github.com/MoAbbasid/roadwork-cone-mapping)

## Visual Document QA

{% include click-gif.html video="/assets/visual-doc-qa-demo-v2.mp4" poster="/assets/visual-doc-qa-poster-v2.jpg" alt="Asking questions about WHO situation reports and an IMF report, each answer shown with its cited page and the value highlighted" w="960" h="567" %}

Point it at a folder of PDFs and ask a question: you get the answer, the page it came from, and the answer value highlighted on that page. Retrieval works on page images, so tables and charts are found as they appear on the page. Everything runs locally on two free Kaggle T4 GPUs, with no API key.

**Stack:** Python, Docling, PyMuPDF, EVIE-4.5B (page-image retrieval), Qwen3-VL-8B (reader), Gradio. Data: WHO Malaysia COVID-19 situation reports, ViDoRe V3.

**Highlights: results** (test questions held out and scored once)

* On the ViDoRe V3 benchmark (human-written reference answers), 58% of answers are judged correct on HR (223 questions) and 62.5% on Finance-EN (216 questions). For context, the ViDoRe V3 paper reports 61–66% (HR) and 59.5–67.3% (Finance-EN) for Qwen3-VL-235B, GPT-5.2 and Gemini 3 Pro.
* 76% exact numeric match on 50 questions about 31 WHO situation reports (155 pages of narrative and tables).
* Page retrieval scores nDCG@10 68.0 (HR) and 72.1 (Finance-EN), reproducing EVIE's published result within a point.

**Code:** [github.com/MoAbbasid/visual-doc-qa](https://github.com/MoAbbasid/visual-doc-qa)
