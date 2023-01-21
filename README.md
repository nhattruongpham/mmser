# mmser
## SERVER: Multi-modal Speech Emotion Recognition using Transformer-based and Vision-based Embeddings
This code is to reproduce the multi-modal speech emotion recognition model that has been used in the paper entitled "SERVER: Multi-modal Speech Emotion Recognition using Transformer-based and Vision-based Embeddings".

### Abstract
This paper proposes a multi-modal approach for speech emotion recognition (SER) using both text and audio inputs. The audio embedding is extracted by using a vision-based architecture, namely VGGish, while the text embedding is extracted by using a transformer-based architecture, namely BERT. Then, these embeddings are fused using concatenation to recognize emotional states. To evaluate the effectiveness of the proposed method, the benchmark dataset, namely IEMOCAP, is employed in this study. Experimental results indicate that the proposed method is very competitive and better than most of the latest and state-of-the-art methods using multi-modal analysis for SER. The proposed method achieves 63.10% unweighted accuracy (UA) and 63.00% weighted accuracy (WA) on the IEMOCAP dataset. In the future, an extension of multi-task learning and multi-lingual approaches will be investigated to improve the performance and robustness of multi-modal SER. For reproducibility purposes, our code is publicly available.

### Dependencies
- Python 3.7
- Pytorch 1.10.0
- Transformer 4.22.0
- TensorboardX 2.5.1
- Pytorch Lightning 1.6.5
- Torchvggish-GPU<sup>[1,2,3]</sup> 0.1

### Usage
Run ```PreState.ipynb``` to train, predict, analyze, and visualize all experimental results in this paper.

### Citation
If you use this code or part of it, please cite the following papers:
```
@inproceedings{DBLP:conf/iciit/PhamDPN23,
  author    = {Nhat Truong Pham and Duc Ngoc Minh Dang and Bich Ngoc Hong Pham and Sy Dzung Nguyen},
  title     = {SERVER: Multi-modal Speech Emotion Recognition using Transformer-based and Vision-based Embeddings},
  booktitle = {{ICIIT} 2023: 8th International Conference on Intelligent Information
               Technology, Da Nang, Vietnam, February 24 - 26, 2023},
  pages     = {},
  publisher = {{ACM}},
  year      = {2023},
  url       = {},
  doi       = {},
  timestamp = {},
  biburl    = {},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### References
<hr>
[1]  S. Hershey et al., ‘CNN Architectures for Large-Scale Audio Classification’,\
    in International Conference on Acoustics, Speech and Signal Processing (ICASSP),2017\
    Available: https://arxiv.org/abs/1609.09430, https://ai.google/research/pubs/pub45611

[2] Harri Taylor et al., ‘Pytorch port of Google Research's VGGish model used for extracting audio features’,
    v0.1, Sep 27, 2019. Available: https://github.com/harritaylor/torchvggish/releases/tag/v0.1

[3] Nhat Truong Pham, ‘torchvggish-gpu’, Sep 29, 2022. Available: https://github.com/nhattruongpham/torchvggish-gpu
