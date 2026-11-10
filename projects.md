---
layout: page
permalink: /projects/index.html
title: Projects
---

# Projects

{% include click-gif-assets.html %}

## Malaysia Seat Analytics

{% include click-gif.html gif="/assets/demo.gif" poster="/assets/malaysia-seat-analytics-poster.jpg" alt="Walkthrough of the Malaysia Seat Analytics dashboard" w="880" h="519" %}

Streamlit dashboard joining open socio-economic data with GE-14 and GE-15 election results across all 222 Malaysian parliamentary constituencies.

**Stack:** Python, pandas, Plotly, Streamlit. Open data from DOSM and ElectionData.MY.

**Key findings:**

* TODO: finding 1
* TODO: finding 2
* TODO: finding 3

**Code available on request.** Contact: TODO

## RoadWork Cone Mapping

{% include click-gif.html gif="/assets/roadwork-cone-mapping-demo.gif" poster="/assets/roadwork-cone-mapping-poster.jpg" alt="Walkthrough of RoadWork Cone Mapping: detected cones with relative gaps, then a Los Angeles route map" w="720" h="422" %}

Cone detection on dashcam frames from the CMU ROADWork dataset, with relative gaps between neighbouring cones and a GPS route map of cone counts along a Los Angeles street.

**Stack:** Python, Ultralytics YOLO26, OpenCV, Folium. Data: CMU ROADWork (ODC-Attribution).

**Key findings:**

* YOLO26s fine-tuned for 50 epochs reaches mAP50 0.747 (precision 0.804, recall 0.717) on the 5,396 cone instances in the validation set.
* Gaps between neighbouring cones are scaled from cone height, assuming a 28 in cone, so they are relative rather than calibrated distances.
* On a 30-frame stretch of Los Angeles, 63 cones were detected and mapped in capture order along the GPS route.

**Code:** [github.com/MoAbbasid/roadwork-cone-mapping](https://github.com/MoAbbasid/roadwork-cone-mapping)
