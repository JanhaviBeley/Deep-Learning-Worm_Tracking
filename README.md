# 🪱 Deep Learning for *C. elegans* Behaviour Analysis

### Computer Vision • Deep Learning • Movement Analysis • Parkinson's Disease Research

> **Applying deep learning and quantitative movement analysis to study *C. elegans* behaviour in the context of Parkinson's disease research.**

---

## Overview

This project explores the use of **deep learning and computer vision to automate *C. elegans* movement tracking and behavioural analysis**.

*C. elegans* is widely used as a model organism in Parkinson's disease research. Quantifying changes in movement can provide measurable behavioural indicators of neurological dysfunction.

The project focuses on converting worm videos into structured movement data and analysing this data to identify meaningful behavioural features.

---
## Research Context

I conducted this work as part of the research at **[LuthLab](https://www.luthlab.org)** , **[Simmons University](https://www.simmons.edu)**, working with **[Dr.Eric Luth](https://www.linkedin.com/in/eric-luth), [Dr.Jared Deighton](https://www.linkedin.com/in/jared-deighton-phd-390362173) and [Dr.Nicole Rockweiler](https://www.linkedin.com/in/nicole-rockweiler)** as my mentors and **[Katie Mendez-Solano](https://www.linkedin.com/in/katie-mendez-solano-5a536421b/)** as the biological researcher.

The project combined biological research with **deep learning, computer vision and data analysis** to study *C. elegans* movement and develop quantitative methods for behavioural analysis relevant to Parkinson's disease research.

- **[LuthLab](https://www.luthlab.org)** 
- **Mentors:** [Dr.Eric Luth](https://www.linkedin.com/in/eric-luth), [Dr.Jared Deighton](https://www.linkedin.com/in/jared-deighton-phd-390362173) and [Dr.Nicole Rockweiler](https://www.linkedin.com/in/nicole-rockweiler). 
- **Research collaborator:** [Katie Mendez-Solano](https://www.linkedin.com/in/katie-mendez-solano-5a536421b/) 

## Research Approach

The overall workflow is:

```text
Video
  ↓
Worm Detection
  ↓
Tracking
  ↓
Skeletonisation
  ↓
Movement Feature Extraction
  ↓
Time-Series & Fourier Analysis
  ↓
Behavioural Interpretation
```

---

## 🔄 From Traditional Tracking to Deep Learning

The analysis progressed from a conventional worm-tracking workflow to a
deep-learning-based approach, followed by quantitative movement analysis.

<p align="center">
  <img src="images/input_video.png" width="28%" />
  &nbsp;→&nbsp;
  <img src="images/wrmtrck.png" width="28%" />
  &nbsp;→&nbsp;
  <img src="images/deep_worm_tracker.png" width="28%" />
</p>

<p align="center">
  <b>Input Video</b>
  &nbsp;&nbsp;→&nbsp;&nbsp;
  <b>Previous Tracking — wrmtrck</b>
  &nbsp;&nbsp;→&nbsp;&nbsp;
  <b>Detection & Tracking — Deep-Worm-Tracker</b>
</p>

<br>

<p align="center">
  <img src="images/tracking_output.png" width="28%" />
  &nbsp;→&nbsp;
  <img src="images/fourier_analysis.png" width="28%" />
  &nbsp;→&nbsp;
  <img src="images/movement_features.png" width="28%" />
</p>

<p align="center">
  <b>Tracking Output</b>
  &nbsp;&nbsp;→&nbsp;&nbsp;
  <b>Movement Frequency Analysis</b>
  &nbsp;&nbsp;→&nbsp;&nbsp;
  <b>Movement Features</b>
</p>
---

## Deep Learning & Computer Vision

I explored **Deep-Worm-Tracker**, which uses YOLO-based object detection and StrongSORT tracking to detect and track *C. elegans* in video data.

The resulting tracking and skeletal information provides a foundation for quantitative movement analysis.

🔗 [Deep-Worm-Tracker](https://github.com/knaticat/Deep-Worm-Tracker)

---

## Movement Analysis

The extracted movement data can be used to investigate features including:

* Body bends
* Movement and speed
* Distance travelled
* Rate of change
* Movement variability
* Amplitude
* Dominant movement frequency

These measurements provide a quantitative representation of behaviour that can complement visual observation.

---

## Fourier Analysis

I used the **Fast Fourier Transform (FFT)** to examine movement signals in the frequency domain.

```text
Movement Signal
      ↓
     FFT
      ↓
Frequency Spectrum
      ↓
Dominant Movement Patterns
```

This provides an additional way to characterise repetitive movement patterns through measures such as **frequency and amplitude**.

---

## Biological Context

The broader aim is to explore whether automated movement analysis can help quantify behavioural phenotypes relevant to **Parkinson's disease research**.

This project brings together:

**Deep Learning + Computer Vision + Data Science + Signal Processing + Biology**

---

## Technologies

**Python** • **NumPy** • **Pandas** • **Matplotlib**
**Deep Learning** • **YOLO** • **StrongSORT**
**Computer Vision** • **Skeletonisation** • **FFT**

---

## 🔒 Code & Data

Source code, raw experimental data and research-specific materials are not publicly available.

This repository serves as a **research showcase**, documenting the methodology, analytical approach and selected non-sensitive visualisations.

---

## Future Work

Potential extensions include:

* Automated body-bend and omega-turn detection
* Curvature and movement analysis
* Behaviour classification using machine learning
* Comparison of behavioural phenotypes
* Integration of multiple movement features

---

## References

**Banerjee, S. C., Khan, K. A., & Sharma, R. (2023).**
*Deep-worm-tracker: Deep learning methods for accurate detection and tracking for behavioral studies in C. elegans.*
Applied Animal Behaviour Science, 266, 106024.

🔗 [Deep-Worm-Tracker](https://github.com/knaticat/Deep-Worm-Tracker)

**Modeling Parkinson's Disease in C. elegans**
🔗 [Research article](https://pmc.ncbi.nlm.nih.gov/articles/PMC5836411/)

---

### 🧠 AI × Biology

**Turning biological movement into measurable data.**
