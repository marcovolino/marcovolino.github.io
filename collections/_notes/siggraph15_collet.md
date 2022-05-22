---
layout: paper
title: 'High-quality streamable free-viewpoint video'
authors: 'Alvaro Collet, Ming Chuang, Pat Sweeney, Don Gillett, Dennis Evseev, David Calabrese, Hugues Hoppe, Adam Kirk, Steve Sullivan'
venue: 'SIGGRAPH'
year: 2015
paper-url: 'https://dl.acm.org/doi/10.1145/2766945'
topic: 'Volumetric Video'
---

## Abstract
We present the first end-to-end solution to create high-quality free-viewpoint video encoded as a compact data stream. Our system records performances using a dense set of RGB and IR video cameras, generates dynamic textured surfaces, and compresses these to a streamable 3D video format. Four technical advances contribute to high fidelity and robustness: multimodal multi-view stereo fusing RGB, IR, and silhouette information; adaptive meshing guided by automatic detection of perceptually salient areas; mesh tracking to create temporally coherent subsequences; and encoding of tracked textured meshes as an MPEG video stream. Quantitative experiments demonstrate geometric accuracy, texture fidelity, and encoding efficiency. We release several datasets with calibrated inputs and processed results to foster future research.

## Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/SkJG-uFU2yA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Notes

**Overview**
- This paper proposes a well engineered, end-to-end system to capture, reconstruct and deliver volumetric video.
- While none of the techniques presented in the paper seem to be particularly novel, they are put together into a practical, comprehensive and state-of-the-art volumetric capture system.
- The results are demonstrated across a wide range of subjects (people, animals, static objects) and the quality is the highest I have seen to date.

**Limitations**:
- Cost: this systems would likely cost several million USD to reproduce and therefore is out of reach to most
- Format: the streamable output format is closed source and should really be made into an open standard

