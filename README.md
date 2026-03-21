# DetReIDX🌍

**DetReIDX: A Stress-Test Dataset for Real-World UAV-Based Person Recognition** (IEEE T-BIOM 2026)
&nbsp;&nbsp;[PDF](https://arxiv.org/pdf/2505.04793)&nbsp;&nbsp;[Project Page](https://www.it.ubi.pt/DetReIDX)&nbsp;&nbsp;[GitHub](https://github.com/kailashhambarde/DetReIDX)&nbsp;&nbsp;[Leaderboard](https://www.it.ubi.pt/DetReIDX/leaderboard.html)

---

### News🔉

- **2026.03.06** — 1st Workshop on [VReID-XFD](https://www.it.ubi.pt/VReID-XFD/) at **WACV 2026**, Tucson, Arizona
- **2026** — Paper accepted at *IEEE Transactions on Biometrics, Behavior, and Identity Science* (T-BIOM)
- **2025.05** — Preprint available on [arXiv](https://arxiv.org/pdf/2505.04793)

---

### Updates👨‍💻

* [X] Build project page
* [X] Person Re-ID split released
* [ ] Person Detection split — Coming Soon
* [ ] Video ReID split — Coming Soon

---

## Teaser🎬

<p align="center">
  <a href="https://www.it.ubi.pt/DetReIDX">
    <img src="https://www.it.ubi.pt/DetReIDX/img/poster_image.png" width="90%"/>
  </a>
</p>
<p align="center"><em>DetReIDX: Long-range person identification from UAV and ground cameras. Click to watch.</em></p>

---

## Dataset: DetReIDX💰

<p align="center">
  <img src="https://www.it.ubi.pt/DetReIDX/img/abstract_figure.jpg" width="100%"/>
</p>
<p align="center"><em>Figure 1: Comparison of DetReIDX with existing datasets across altitude coverage, annotation richness, and task support.</em></p>

---

### Highlights💴

- **509 unique identities** | **13M+ bounding box annotations** | **7 international collection sites**
- **18 UAV viewpoints per subject** — altitudes 5m to 120m, distances 10m to 120m, pitch angles 30°/60°/90°
- **Clothing variation across sessions** — tests long-term identity persistence
- **16 soft biometric attributes** per frame — demographics, appearance, clothing, action
- **4 tasks**: Person Detection · Re-ID · Multi-View Tracking · Action Recognition

### Settings♻️

| Setting | Environment | Altitude | Distance | Data Type |
|---------|-------------|----------|----------|-----------|
| **Indoor** | University Labs | Ground level | Close range | Profile images, gait videos |
| **Outdoor** | University Campuses | 5–120m | 10–120m | Multi-view videos, action clips |

| Indoor Lab Setup | Outdoor UAV Setup |
|:----------------:|:-----------------:|
| ![Indoor](https://www.it.ubi.pt/DetReIDX/figures/indoor_settigs.jpg) | ![Outdoor](https://www.it.ubi.pt/DetReIDX/figures/outdoor_setup.jpg) |

### Examples📹

**Teaser:** [intro2.mp4](https://www.it.ubi.pt/DetReIDX/videos/teaser/intro2.mp4)

**Outdoor UAV Examples:**

| Site | Video |
|------|-------|
| Istanbul Medipol University | [Watch](https://www.it.ubi.pt/DetReIDX/videos/outdoor_examples/gokhan.mp4) |
| JNNCE, India | [Watch](https://www.it.ubi.pt/DetReIDX/videos/outdoor_examples/pawankumar.mp4) |
| SRMIST, India | [Watch](https://www.it.ubi.pt/DetReIDX/videos/outdoor_examples/srm.mp4) |
| SRTMUN, India | [Watch](https://www.it.ubi.pt/DetReIDX/videos/outdoor_examples/srtmun.mp4) |
| University of Luanda, Angola | [Watch](https://www.it.ubi.pt/DetReIDX/videos/outdoor_examples/angola.mp4) |
| NMDC | [Watch](https://www.it.ubi.pt/DetReIDX/videos/outdoor_examples/pawanwasnik.mp4) |

**Indoor Reference Session:** [indoor_sample_video.mp4](https://www.it.ubi.pt/DetReIDX/videos/indoor_examples/indoor_sample_video.mp4)

### Attributes📋


| # | Attribute | Values |
|---|-----------|--------|
| 1 | Gender | Male, Female, Unknown |
| 2 | Age | 0–11, 12–17, 18–24, 25–34, 35–44, 45–54, 55–64, >65, Unknown |
| 3 | Height | Child, Short, Medium, Tall, Unknown |
| 4 | Body Volume | Thin, Medium, Fat, Unknown |
| 5 | Ethnicity | White, Black, Asian, Indian, Unknown |
| 6 | Hair Color | Black, Brown, White, Red, Gray, Occluded, Unknown |
| 7 | Hairstyle | Bald, Short, Medium, Long, Ponytail, Unknown |
| 8 | Beard | Yes, No, Unknown |
| 9 | Moustache | Yes, No, Unknown |
| 10 | Glasses | Normal, Sun, No, Unknown |
| 11 | Head Accessories | Hat, Scarf, Necklace, Cannot see, Unknown |
| 12 | Upper Body Clothing | T-Shirt, Blouse, Sweater, Coat, Dress, Uniform, Shirt, Suit, Hoodie, Cardigan, Unknown |
| 13 | Lower Body Clothing | Jeans, Leggings, Pants, Shorts, Skirt, Dress, Uniform, Suit, Unknown |
| 14 | Feet | Sport Shoe, Classic Shoe, High Heels, Boots, Sandal, Nothing, Unknown |
| 15 | Accessories | Bag, Backpack, Rolling Bag, Umbrella, Sport Bag, Market Bag, Nothing, Unknown |
| 16 | Action | Walking, Running, Standing, Sitting, Cycling, Exercising, Talking on Phone, and more |

Full encoding details: [soft_bio_readme.md](soft_bio_readme.md)

---

## Download💾

Files are distributed as **password-protected ZIP** archives.
After downloading, email with your *name*, *institution*, and *intended use* to receive the password.

📧 [n1947@ubi.pt](mailto:n1947@ubi.pt) or [kailas.srt@gmail.com](mailto:kailas.srt@gmail.com) — Subject: *"DetReIDX Password Request"*

| Split | Status | Link |
|-------|--------|------|
| **Person Re-ID** (still + video, with attribute labels) | ✅ Available | [Google Drive](https://drive.google.com/file/d/1TZ0-CJ05ANSkM2RsD6IPGaZ0qThoQNsp/view?usp=sharing) |
| **Person Detection** (bounding box annotations) | 🕐 Coming Soon | — |
| **Video ReID** (multi-session tracklets) | 🕐 Coming Soon | — |

[📄 Download License Agreement (PDF)](https://www.it.ubi.pt/DetReIDX/DetReIDX_Dataset_License_Terms_and_Access_Request_Form.pdf)

---

## Folder Structure📂

```
DetReIDX/
├── train/
│   └── <PID>/
│       └── <tracklet>/
│           └── *.jpg
├── query/
│   └── <PID>/
│       └── <tracklet>/
│           └── *.jpg
└── gallery/
    └── <PID>/
        └── <tracklet>/
            └── *.jpg
```

---

## Evaluation Protocols📊

| Protocol | Task | Metric |
|----------|------|--------|
| Short-Term ReID | Match within same session | mAP, CMC Rank-1/5/10 |
| Long-Term ReID | Match across sessions (clothing change) | mAP, CMC Rank-1/5/10 |
| Cross-View ReID | Aerial ↔ Ground matching | mAP, CMC Rank-1/5/10 |
| Detection | Pedestrian bounding box prediction | mAP@0.5, mAP@0.75 |
| Tracking | Multi-view person tracking | MOTA, IDF1 |

Full experimental results (YOLOv8, DDOD, Grid-RCNN, PersonViT, SeCap, CLIP-ReID) in the [paper](https://arxiv.org/pdf/2505.04793).

---

## Acknowledgement🏫

We acknowledge and give credit to the following universities for their contributions:
**Istanbul Medipol University · J.N.N College of Engineering · SRM Institute of Science and Technology · Swami Ramanand Teerth Marathwada University Nanded · Universidade Beira Interior · Universidade de Luanda** *(A–Z)*

<p align="center">
  <img src="https://www.it.ubi.pt/DetReIDX/img/logos.png" width="90%"/>
</p>

---

## Citation📝

```bibtex
@article{hambarde2026detreidx,
  title     = {DetReIDX: A Stress-Test Dataset for Real-World UAV-Based Person Recognition},
  author    = {Hambarde, Kailash A and Mbongo, Nzakiese and Kumar, MP Pavan and Mekewad, Satish
               and Fernandes, Carolina and Silahtaro{\u{g}}lu, G{\"o}khan and Nithya, Alice
               and Wasnik, Pawan and Rashidunnabi, MD and Samale, Pranita and others},
  journal   = {IEEE Transactions on Biometrics, Behavior, and Identity Science},
  year      = {2026},
  publisher = {IEEE}
}
```

---

## License

Released for **academic and non-commercial use only**. By downloading or using this dataset, you agree to the terms on the [project website](https://www.it.ubi.pt/DetReIDX).
