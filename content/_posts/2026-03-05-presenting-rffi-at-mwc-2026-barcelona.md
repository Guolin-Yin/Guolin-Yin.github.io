---
layout: post
title: "Presenting Cross-Environment Wi-Fi RFFI at Mobile World Congress 2026 Barcelona"
date: 2026-03-05
description: "Showcasing our real-time Wi-Fi based Radio Frequency Fingerprint Identification system at MWC 2026, demonstrating cross-environment robustness with over 90% accuracy"
tags: [RFFI, MWC, conference, HASC, wireless-security, demo]
categories: [events, research]
published: true
toc:
  beginning: true
---

## Introduction

I had the incredible opportunity to present our **real-time Wi-Fi based Radio Frequency Fingerprint Identification (RFFI)** work at **Mobile World Congress (MWC) 2026** in Barcelona, representing the **[Hub in All-Spectrum Connectivity (HASC)](https://allspectrumhub.org/)**. This prestigious event provided an excellent platform to demonstrate how our RFFI system achieves robust device identification across diverse and previously unseen environments.

## The HASC Hub

The **Hub in All-Spectrum Connectivity (HASC)** is a major UK research initiative based at the University of Oxford, supported by EPSRC (UK Research and Innovation) and the Department of Science, Innovation and Technology. HASC brings together leading researchers from:

- **University of Oxford** (Lead)
- **University of Cambridge** (Security challenge)
- **University College London** (Connectivity challenge)
- **University of Bristol** (Adaptivity challenge)
- **Queen's University Belfast**

Our RFFI work contributes to the **Security challenge (C3)**, led by the University of Cambridge, focusing on ensuring that future communication networks remain secure and resilient.

## Our Demo at MWC 2026

At the HASC Hub exhibition booth, we showcased our **cross-environment Wi-Fi RFFI system** that can identify wireless devices based on their unique hardware characteristics. The key innovation is the system's ability to maintain high accuracy even in environments completely different from where it was trained.

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/posts/mwc2026/IMG_6499.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Presenting the RFFI demo at the HASC Hub booth, MWC 2026 Barcelona</div>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/posts/mwc2026/IMG_8075.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Live demonstration of real-time device identification</div>
  </div>
</div>

## Cross-Environment Robustness: The Key Challenge

Traditional RFFI systems often suffer significant performance degradation when deployed in environments different from their training conditions. Factors such as:

- **Multipath propagation patterns**
- **Signal interference**
- **Physical obstructions**
- **Distance variations**

All contribute to channel-induced distortions that can mask the subtle hardware fingerprints we rely on for identification.

## Results at MWC 2026

Over the **five days** of Mobile World Congress, our system processed **over 52,000 inference packets** in real-time, achieving an **overall accuracy of 92%**. This is particularly significant because:

- The **radio environment at MWC was far more challenging** than typical daily life or laboratory settings
- The exhibition hall was densely packed with thousands of wireless devices, access points, and electronic equipment creating significant interference
- The model, trained at the **University of Liverpool**, had never seen this environment before
- Despite these harsh conditions, the system maintained robust cross-environment performance

This real-world deployment demonstrates that our RFFI system can generalize effectively to completely unknown and highly challenging radio environments.

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/posts/mwc2026/IMG_8023.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">Explaining the cross-environment methodology to MWC attendees</div>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/posts/mwc2026/IMG_8013.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
    <div class="caption">The complete RFFI demonstration setup at MWC</div>
  </div>
</div>

## System Architecture

Our real-time demonstration system consists of:

- **Transmitters**: Multiple Wi-Fi dongles (9 devices across 3 brands)
- **Receiver**: USRP N210 Software Defined Radio
- **Processing**: Linux laptop running our pretrained deep learning model
- **User Interface**: Real-time visualization of device identification results

The system captures Wi-Fi signals, extracts RF fingerprint features, and performs device classification in real-time, demonstrating the practical viability of RFFI for real-world deployments.

## Key Takeaways from MWC 2026

Presenting at MWC provided valuable insights:

1. **Industry Interest**: Strong interest from telecommunications companies in physical layer security solutions
2. **Practical Deployment**: Questions focused on scalability and integration with existing infrastructure
3. **Standardization**: Discussions about the need for standardized RFFI evaluation frameworks
4. **Future Applications**: Potential applications in 5G/6G security, IoT authentication, and enterprise networks

## Acknowledgments

This work was supported by the **Hub in All-Spectrum Connectivity (HASC)**, funded by EPSRC and the UK Department of Science, Innovation and Technology. Special thanks to the HASC team for organizing the exhibition and to everyone who visited our booth to learn about RFFI technology.

## Looking Forward

The successful demonstration at MWC 2026 validates that cross-environment RFFI is moving from research to practical deployment. Future work will focus on:

- Scaling to larger device populations
- Integration with 6G network architectures
- Addressing open-set recognition challenges
- Federated learning approaches for privacy-preserving training

---

For more details about the technical implementation, please visit the [Real-time Wi-Fi based RFFI project page](/projects/Real-time%20Wi-Fi%20based%20RFFI/).
