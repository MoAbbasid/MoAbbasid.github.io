---

layout: page

---

# About Me

I'm a Graduate Research Assistant pursuing a Master's in Information Technology at [Multimedia University Malaysia](https://www.mmu.edu.my). Currently immersed in applied AI for infrastructure inspect[...]


## Research Interests

* Practical AI for telecom infrastructure and safety assessment
* Visual representation learning and contrastive methods
* Vision–language models (CLIP, BLIP) and few-shot adaptation
* Detection models and feature extraction (YOLO, SSD and backbones)
* Occlusion evaluation, Synthetic imagegeneration, and augmentation
* Embedding-based retrieval and classification with limited labels
* Graph neural networks for spatial/contextual reasoning


---

## Publications

* **Deep Learning Based Utility Pole Safety Assessment from Visual Data**
  Presents a YOLO-based detection baseline and an initial safety assessment pipeline for utility pole images.
  Publisher page: [Article](https://joiv.org/index.php/joiv/article/view/3039)

* **Feature-Based Utility Pole Assessment under Occlusion Using Detection and Vision-Language Models**
(in preparation).  
Compares feature representations from a detection model (YOLO) and a vision–language model (CLIP) for utility pole image assessment under varying levels of visual occlusion. Evaluates which representation is most robust.

---

## Blog Posts

<ul>
{% for post in site.posts %}
  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

<br>
