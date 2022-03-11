---
title: "Video Frame Interpolation"
disableToc: false 
---

## Resources
- The goal of **Video Frame Interpolation** is to synthesize several frames in the middle of two adjacent frames of the original video. Video Frame Interpolation can be applied to generate slow motion video, increase video frame rate, and frame recovery in video streaming.

## References
- #PAPER [Asymmetric Bilateral Motion Estimation for Video Frame Interpolation (Park 2021)](https://arxiv.org/abs/2108.06815)
	- https://github.com/JunHeum/ABME
- #PAPER [Enhanced Correlation Matching based Video Frame Interpolation (Lee 2021)](https://arxiv.org/abs/2111.08869v1)
- #PAPER [FILM: Frame Interpolation for Large Motion (Reda 2022)](https://arxiv.org/abs/2202.04901v2)
	- #CODE https://github.com/google-research/frame-interpolation
	- https://www.youtube.com/watch?v=OAD-BieIjH4
	- present a single unified network, distinguished by a multi-scale feature extractor that shares weights at all scales, and is trainable from frames alone
	- to synthesize crisp and pleasing frames, proposed to optimize the network with the Gram matrix loss that measures the correlation difference between feature maps