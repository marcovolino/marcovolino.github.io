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


## Notes

This paper proposes a well engineered, comprehensive system to capture, reconstruct and deliver volumetric video.

While none of the techniques presented in the paper are novel in themselves, the combination of them to create a state of the art volumetric capture system is novel.


The quality of the output is the highest to date that I have seen

Limitations:
- Cost: this systems would likely cost several million to reproduce
- Format: the streamable format is not an open standard
