---
layout: page
title: Real-time Wi-Fi based RFFI
description: Cross-environment WiFi based RFFI
img: assets/img/RFFI_DEMO/setup.jpg
importance: 1
category: demo
related_publications: true
---
This project aims to achieve a cross-environment Wi-Fi based RFFI prototype. The signal collection is based on Picoscenes

## Overall Setup

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/setup.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Overall system setup of the real-time Wi-Fi based RFFI demo</div>
  </div>
</div>



## Real-time Wi-Fi based RFFI Demo

This project demonstrates a real-time, cross-environment Wi-Fi-based Radio Frequency Fingerprint Identification (RFFI) prototype. The system is designed to identify physical devices based on their unique RF characteristics using deep learning.

### System Overview

The demo setup consists of the following components:

- **User Interface (UI):**  
  A dedicated UI allows users to interact with the demo system, visualize results, and control the identification process.
  <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/ui.png" class="img-fluid rounded z-depth-1" %}


- **Access Point (AP):**  
  The AP is responsible for connecting multiple Wi-Fi dongles (transmitters) to the network, enabling communication and data collection.
  <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/ap.png" class="img-fluid rounded z-depth-1" %}


- **Transmitter:**  
  A laptop equipped with a Wi-Fi dongle acts as the transmitter, sending Wi-Fi packets for identification.
  <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/transmitter_laptop.png" class="img-fluid rounded z-depth-1" %}


- **Receiver:**  
  The receiver is implemented using a USRP (Universal Software Radio Peripheral), which captures the Wi-Fi signals transmitted by the dongles.
  <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/usrpn210.png" class="img-fluid rounded z-depth-1" %}

- **Processor:**  
  The USRP is connected to a Linux laptop that serves as the processing unit. This processor runs a pretrained neural network model, which performs real-time identification of the physical devices based on their RF fingerprints.
  <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
      {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/proccesor.png" class="img-fluid rounded z-depth-1" %}

## Experiment Setup

- **Training environment:** Office
- **Distance (training):** 1 meter between transmitter and receiver
- **Number of devices:** 9
- **Brands:** Three (Device A, Device B, Device C)
- **Dongles per brand:** 3 (total 9 dongles)
- **Testing:** Performed in various environments and distances to evaluate generalization
- **Confusion matrices:** Results for each test scenario are shown below. The filename indicates the environment and distance.

| Environment    | Distance(s)      | Scenario             | Special Notes         |
|---------------|------------------|----------------------|----------------------|
| Office        | 1m, 5m           | In-environment       | Training at 1m       |
| Classroom     | 1m, 10m          | Cross-environment    |                      |
| Meeting Room  | 1m, 3m, NOLS     | Cross-environment    | NOLS = No Line of Sight |

The dataset for both training and testing was collected across multiple months to ensure robustness and account for temporal variations.

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Office-1m.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Office, 1m (Training Environment)</div>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Office-5m.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Office, 5m</div>
  </div>
</div>
<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Classroom_1m.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Classroom, 1m</div>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Classroom_10m.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Classroom, 10m</div>
  </div>
</div>
<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Meeting_room_1m.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Meeting Room, 1m</div>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Meeting_room_3m.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Meeting Room, 3m</div>
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/RFFI_DEMO/Results/Meeting_room_NOLS.jpg" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Meeting Room, No Line of Sight</div>
  </div>
</div>

## Demo Video in Meeting room environment

<div style="position: relative; width: 100%; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe src="https://www.youtube.com/embed/jQuvRcBXh8I"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allowfullscreen
          class="rounded z-depth-1 mb-4"></iframe>
</div>
<div class="caption">
    Demo video for the real-time Wi-Fi based RFFI system.
</div>