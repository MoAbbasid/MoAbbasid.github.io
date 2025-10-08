---

layout: page

---

# About Me

I'm a Graduate Research Assistant pursuing a Master's in Information Technology at [Multimedia University Malaysia](https://www.mmu.edu.my). Currently immersed in applied AI for infrastructure inspection, my thesis is **Utility Pole Safety Assessment from Visual Data’**. At [Telekom Malaysia R&D](https://www.tmrnd.com.my), I implemented computer vision models and evaluate their performance for practical safety tasks. Previously, as a Full Stack Developer in the telecom industry, I developed microservices and APIs. I aim to bridge academic research with real-world engineering impact.


## Research Interests

* Image Information Retrieval
* Practical AI for telecom infrastructure and safety assessment
* Visual representation learning and contrastive methods
* Vision–language models (CLIP, BLIP) and few-shot adaptation
* Detection models and feature extraction (YOLO, SSD and backbones)
* Occlusion evaluation, Synthetic image generation, and augmentation
* Embedding-based retrieval and classification with limited labels
* Graph neural networks for spatial/contextual reasoning


---

## Publications

* **Deep Learning Based Utility Pole Safety Assessment from Visual Data**
Designed an AI-driven solution to automatically detect utility poles and evaluate safety clearance violations, addressing challenges in costly and subjective manual inspections. Built and augmented a custom dataset and achieved 83% compliance classification accuracy with YOLOv8 as the backbone, enabling reliable large-scale infrastructure safety monitoring. [Article](https://joiv.org/index.php/joiv/article/view/3039)

* **Feature-Based Utility Pole Assessment under Occlusion Using Detection and Vision-Language Models**
(in preparation).  
Compares feature representations from a detection model (YOLO) and a vision–language model (CLIP) for utility pole image assessment under varying levels of visual occlusion. Evaluates which representation better supports downstream classification and retrieval with limited labeled data.

---

## Blog Posts

<ul>
{% for post in site.posts %}
  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

<br>
