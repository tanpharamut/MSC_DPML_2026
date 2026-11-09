# MSC_DPML_2026

คลังเอกสารรายวิชา **MSC_DPML_2026** — สไลด์เลกเชอร์ การบ้าน ควิซ สรุปบทเรียน
และงานวิจัยส่วนตัว รวบรวมไว้ที่เดียว

**ปรมัตถ์ มากเจริญ · 6950200196**

---

## เริ่มตรงไหนดี

| อยากได้อะไร | ไปที่ |
|---|---|
| เกณฑ์คะแนนและไทม์ไลน์ของวิชา | [`01-course-info/course-info.md`](01-course-info/course-info.md) |
| สไลด์ที่อาจารย์สอนในห้อง | [`02-lectures/`](02-lectures/) |
| สรุปอ่านทบทวนก่อนสอบ | [`03-notes/`](03-notes/) |
| การบ้าน HW1–HW4 | [`04-homework/`](04-homework/) |
| งานควิซที่ส่งไปแล้ว | [`05-quizzes/`](05-quizzes/) |
| Research Project (Deepfake) | [`06-project/`](06-project/) |

---

## โครงสร้างโฟลเดอร์

```
MSC_DPML_2026/
├── 01-course-info/        เกณฑ์คะแนน + ไทม์ไลน์
├── 02-lectures/           สไลด์เลกเชอร์ แยกตามหัวข้อ
│   ├── 01-ai-foundations/
│   ├── 02-data-preprocessing/
│   ├── 03-image-preprocessing/
│   └── 04-text-preprocessing/
├── 03-notes/              สรุปบทเรียนแบบ HTML อ่านในเบราว์เซอร์
├── 04-homework/           การบ้าน แยกเป็น hw1–hw4
│   ├── hw1-research-topic/
│   ├── hw2-title-abstract/
│   ├── hw3-deepfake-papers/
│   └── hw4-group-k-fold/
├── 05-quizzes/            งานควิซ
└── 06-project/            Research Project
```

ทุกโฟลเดอร์ย่อยของการบ้านใช้รูปแบบเดียวกัน คือมีไฟล์นำเสนอ (`presentation-YYYY-MM-DD`)
อยู่ชั้นนอก และเปเปอร์ที่ใช้อ้างอิงอยู่ใน `papers/`

---

## 02 · สไลด์เลกเชอร์

| หัวข้อ | ไฟล์ | หน้า |
|---|---|---:|
| พื้นฐาน AI | [`ai-1.0.2.pdf`](02-lectures/01-ai-foundations/ai-1.0.2.pdf) | 9 |
| การเตรียมข้อมูล ตอนที่ 1 | [`preprocessing-part1.pdf`](02-lectures/02-data-preprocessing/preprocessing-part1.pdf) | 25 |
| การเตรียมข้อมูล ตอนที่ 2 | [`preprocessing-part2.pdf`](02-lectures/02-data-preprocessing/preprocessing-part2.pdf) | 25 |
| ภาพดิจิทัลเกิดขึ้นได้อย่างไร | [`class1-how-a-digital-image-is-formed.pdf`](02-lectures/03-image-preprocessing/class1-how-a-digital-image-is-formed.pdf) | 130 |
| เตรียมภาพก่อนและระหว่าง train | [`class2-preprocessing-before-and-during-training.pdf`](02-lectures/03-image-preprocessing/class2-preprocessing-before-and-during-training.pdf) | 104 |
| เตรียมข้อความแบบดั้งเดิม | [`textclass1-classical-preprocessing.pdf`](02-lectures/04-text-preprocessing/textclass1-classical-preprocessing.pdf) | 128 |
| เตรียมข้อความในยุค LLM | [`textclass2-llm-era-preprocessing.pdf`](02-lectures/04-text-preprocessing/textclass2-llm-era-preprocessing.pdf) | 165 |

---

## 03 · สรุปบทเรียน

ไฟล์ HTML เปิดอ่านได้ในเบราว์เซอร์โดยตรง ไม่ต้องติดตั้งอะไรเพิ่ม

| ไฟล์ | เนื้อหา |
|---|---|
| [`msc26-ai-notes.html`](03-notes/msc26-ai-notes.html) | สรุปภาพรวมวิชา — AI คืออะไร, LLM เรียนรู้ยังไง, Pre-training → SFT → RLHF, RAG, Agentic AI, CRISP-DM, การแบ่ง fold, imbalanced data, ensemble |
| [`msc26-slide-guide.html`](03-notes/msc26-slide-guide.html) | คู่มือไล่ทีละสไลด์ — เซนเซอร์และการเกิดภาพ, sampling/quantization, aliasing, color space, resize, bit depth, CT windowing, filtering, normalization, augmentation, การเตรียมข้อความ |

---

## 04 · การบ้าน

| งาน | วันนำเสนอ | หัวข้อ | เปเปอร์ |
|---|---|---|---:|
| [HW1](04-homework/hw1-research-topic/) | 30 มิ.ย. 2026 | เสนอหัวข้อ Research Project + AI Ethics | 4 |
| [HW2](04-homework/hw2-title-abstract/) | 2 ก.ค. 2026 | นำเสนอ Title–Abstract | 3 |
| [HW3](04-homework/hw3-deepfake-papers/) | 4 ส.ค. 2026 | เปเปอร์ Deepfake Detection | 6 |
| [HW4](04-homework/hw4-group-k-fold/) | ส.ค. 2026 | Group K-Fold แบบกัน identity/video leakage | — |

HW1 และ HW2 ใช้หัวข้อ **Cervical Vertebral Maturation (CVM)**
ส่วน HW3 เป็นต้นไปเปลี่ยนมาเป็น **Deepfake Detection** ซึ่งต่อยอดเป็น Research Project

<details>
<summary><b>เปเปอร์ของ HW1 — Cervical Vertebral Maturation</b></summary>

| ไฟล์ | ชื่อเต็ม |
|---|---|
| `cvm-ai-accuracy-systematic-review.pdf` | Accuracy of Artificial Intelligence for Cervical Vertebral Maturation: A Systematic Review |
| `cvm-ai-algorithm-stage-assessment.pdf` | Artificial intelligence-based algorithm for cervical vertebrae maturation stage assessment |
| `cvm-ml-techniques-literature-review.pdf` | Cervical Vertebral Maturation Assessment using various Machine Learning techniques on Lateral cephalogram: A systematic literature review |
| `cvm-deep-learning-pubertal-growth-pilot.pdf` | Deep learning for the classification of cervical maturation degree and pubertal growth spurts: A pilot study |

</details>

<details>
<summary><b>เปเปอร์ของ HW2 — Cervical Vertebral Maturation</b></summary>

| ไฟล์ | ชื่อเต็ม |
|---|---|
| `cvm-ai-automatic-classification-stages.pdf` | An Artificial Intelligence Model for the Automatic Classification of the Cervical Vertebral Maturation Stages |
| `cvm-llm-comparative-performance.pdf` | Comparative performance analysis of AI-based large language models in assessing cervical vertebral maturation stages on lateral cephalometric radiographs |
| `cvm-ml-determination-lateral-ceph.pdf` | Determination of cervical vertebral maturation using machine learning in lateral cephalograms |

</details>

<details>
<summary><b>เปเปอร์ของ HW3 — Deepfake Detection</b></summary>

| ไฟล์ | ชื่อเต็ม |
|---|---|
| `deepfakebench-comprehensive-benchmark.pdf` | DeepfakeBench: A Comprehensive Benchmark of Deepfake Detection |
| `preserving-fairness-generalization-cvpr2024.pdf` | Preserving Fairness Generalization in Deepfake Detection (CVPR 2024) |
| `deepfake-detection-generalizes-wacv2026.pdf` | Deepfake Detection that Generalizes Across Benchmarks (WACV 2026) |
| `mevit-meta-learning-efficientnet-vit.pdf` | MEViT: Generalization of Deepfake Detection With Meta-Learning EfficientNet Vision Transformer |
| `aasist3-kan-speech-deepfake-ssl.pdf` | AASIST3: KAN-Enhanced AASIST Speech Deepfake Detection using SSL |
| `scalable-aasist-graph-attention.pdf` | Towards Scalable AASIST: Refining Graph Attention |

</details>

### HW4 — Group K-Fold

แบ่ง fold ของชุดข้อมูล AI Face Images โดยกัน **identity / video leakage**:
รูปหลายรูปที่มาจากคนหรือคลิปเดียวกันต้องอยู่ fold เดียวกัน ไม่งั้นโมเดลจะ "จำหน้า"
แทนที่จะเรียนลักษณะ real/fake จริง

- ใช้ `StratifiedGroupKFold` 10 folds, `random_state=42`
- ดึง group key จาก `Image Path` ด้วย regex แยกตามชุดข้อมูลย่อย (DCFACe, Celeb-DF, FF++, IMDb-WiKi)
- Stratify ตาม `Target` (real / fake)

| โฟลเดอร์ | เนื้อหา |
|---|---|
| [`notebooks/`](04-homework/hw4-group-k-fold/notebooks/) | 5 เวอร์ชัน v1 → v5 (v5 คือเวอร์ชันล่าสุด) |
| [`data/`](04-homework/hw4-group-k-fold/data/) | CSV ต้นทาง — **ไม่อยู่ใน Git** ดูรายละเอียดใน [`data/README.md`](04-homework/hw4-group-k-fold/data/README.md) |

---

## 05 · ควิซ

| ไฟล์ | เนื้อหา |
|---|---|
| [`2026-08-25-gaussian-filter-worksheet.pdf`](05-quizzes/2026-08-25-gaussian-filter-worksheet.pdf) | งานเขียนมือ — คำนวณน้ำหนัก Gaussian kernel (อัตราส่วน 1:2:4, ผลรวม 16) |
| [`2026-09-24-quiz2-perceptron.png`](05-quizzes/2026-09-24-quiz2-perceptron.png) | Quiz 2 — เทรน Perceptron 5 epoch ด้วยมือ พร้อมคำนวณ Accuracy / Precision / Recall / Specificity |

---

## 06 · Research Project

หัวข้อ **Deepfake Detection** ต่อยอดจากเปเปอร์ใน HW3

| ไฟล์ | เนื้อหา |
|---|---|
| [`pg-fdd-story-v13-2026-10-22.pptx`](06-project/pg-fdd-story-v13-2026-10-22.pptx) | สไลด์เล่าเรื่องงานวิจัย PG-FDD เวอร์ชัน 13 (22 ต.ค. 2026) |
| [`deepfake-detection-model-groups.jpg`](06-project/deepfake-detection-model-groups.jpg) | ภาพสรุปโมเดล 5 ตัว แบ่งเป็นกลุ่มภาพ/วิดีโอ และกลุ่มเสียง |

---

## หมายเหตุ

- ไฟล์ CSV ของ HW4 (รวมประมาณ 126 MB) ไม่ได้อยู่ใน repo เพื่อไม่ให้ขนาด repo
  บวมเกินจำเป็น — อยู่ใน `.gitignore` และมีคำอธิบายวิธีวางไฟล์ใน `data/README.md`
- สไลด์เลกเชอร์ทุกไฟล์เป็นต้นฉบับความละเอียดเต็ม (ไม่ได้บีบอัด)
