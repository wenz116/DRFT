# End-to-end Multi-modal Video Temporal Grounding

[[Paper]](https://arxiv.org/abs/2107.05624)

PyTorch implementation of our method for identifying the time interval of a certain event in a video based on a natural language description.

Contact: Yi-Wen Chen (ychen319@ucmerced.edu)

## Introduction

Text-guided video temporal grounding aims to identify the time interval of certain events based on natural language descriptions. Different from most existing methods that only consider RGB images as visual features, we propose a multi-modal framework to extract complementary information from videos. Specifically, we adopt **RGB images** for appearance, **optical flow** for motion, and **depth maps** for image structure. While RGB images provide abundant visual cues of certain event, the performance may be affected by background clutters. Therefore, we use optical flow to focus on large motion and depth maps to infer the scene configuration when the action is related to objects recognizable with their shapes.

To integrate the three modalities more effectively and enable inter-modal learning, we design a dynamic fusion scheme with transformers to model the interactions between modalities. Furthermore, we apply intra-modal self-supervised learning to enhance feature representations across videos for each modality, which also facilitates multi-modal learning.

We conduct extensive experiments on the Charades-STA and ActivityNet Captions datasets, and show that the proposed method performs favorably against state-of-the-art approaches.

## Paper

[End-to-end Multi-modal Video Temporal Grounding](https://arxiv.org/abs/2107.05624) <br />
[Yi-Wen Chen](https://wenz116.github.io/), [Yi-Hsuan Tsai](https://sites.google.com/site/yihsuantsai/home), and [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/index.html) <br />
*Neural Information Processing Systems (NeurIPS)*, 2021 <br />

Please cite our paper if you find it useful for your research.

```
@inproceedings{Chen_DRFT_2021,
  author = {Yi-Wen Chen and Yi-Hsuan Tsai and Ming-Hsuan Yang},
  journal = {Neural Information Processing Systems (NeurIPS)},
  title = {End-to-end Multi-modal Video Temporal Grounding},
  year = {2021}
}
```

Codes will be released soon.
