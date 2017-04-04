---
layout: page
title: Projects
excerpt: "Ongoing and recent academic and research projects."
modified: 2016-09-12T08:42:37-04:00
image:
  feature: projects_splash.jpg
---

Here are some things I am working on. Feel free to contact me 

* Table of Contents
{:toc}

## Monitoring urban acoustic environments with acoustic arrays

I am beginning to design and prototype low-cost, low-power acoustic arrays that can be deployed on urban rooftops. The goal is to characterize the acoustic environment of urban areas above the urban canyon. What can we learn about a city with a network of these? Can we estimate bird species biodiversity, population counts, and migration habits?

---

## Processing acoustic array data on the Qualcomm Snapdragon

Using the popular mobile processor, I am implementing a real-time conventional beamformer for a microphone array. With an on-board, programmable DSP unit and GPU, the Snapdragon processor is perfect for signal processing workloads. I hope to show that this mobile processor, when programmed efficiently, can handle the computation-heavy work of array processing and as such is a strong candidate of processor for future embedded array processing projects.

---

## Capturing microphone array data from the NIST MK3

For acoustic array data capture, I have outfitted a Raspberry Pi with the network configuration and automatic data capture needed to interface with a NIST MK3 microphone array. When the recording service is started, the service will automatically detect a USB drive and start recording audio data to it!

---

## Classifying land-use along the I-85 corridor

Using the spectral bands of Landsat 8 I built a simple euclidean distance classifier to identify the land-use type of each pixel. By automating much of the data acquisition, ground-truth mask generation and Landsat data pre-processing I was able to see how this classifier and the spectral data it relied on exhibited strong seasonality and even the short-term variations that caused classification errors. The code for this project is available on my Github [here](https://github.com/anil-ganti/land-use-classify)

---
