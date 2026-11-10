---
layout: page
permalink: /projects/roadwork-cone-mapping/index.html
title: RoadWork Cone Mapping
---

# RoadWork Cone Mapping

[&larr; Back to projects](/projects/index.html)

Cones detected on dashcam frames from the CMU ROADWork dataset and mapped along a GPS route in Los Angeles: 30 consecutive frames, 63 cones. Each dot is one frame, coloured by how many cones were detected in it: grey for none, yellow for 1-3, orange for 4-8 and red for 9 or more.

## Route in capture order

Press play to watch the route build from the first frame to the last. Click a dot to see its cone count.

<iframe src="/assets/maps/route_map_los_angeles_A.html" title="Los Angeles route map, built in capture order" loading="lazy" style="width:100%;height:520px;border:1px solid #bbb;"></iframe>

[Open this map in its own tab](/assets/maps/route_map_los_angeles_A.html)

## Direction of travel

The moving dashes show which way the vehicle travelled. Hover over a dot to see its frame number and cone count.

<iframe src="/assets/maps/route_map_los_angeles_B.html" title="Los Angeles route map, moving dashes show direction of travel" loading="lazy" style="width:100%;height:520px;border:1px solid #bbb;"></iframe>

[Open this map in its own tab](/assets/maps/route_map_los_angeles_B.html)

## About

YOLO26s fine-tuned on ROADWork cone annotations reaches mAP50 0.747 on the validation set. Code, results and the full write-up: [github.com/MoAbbasid/roadwork-cone-mapping](https://github.com/MoAbbasid/roadwork-cone-mapping).

Data: ROADWork dataset (Carnegie Mellon University), ODC Attribution License. Map tiles: &copy; OpenStreetMap contributors.
