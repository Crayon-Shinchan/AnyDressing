<div align="center">

  <h1 align="center">[CVPR 2025]AnyDressing: Customizable Multi-Garment Virtual Dressing via Latent Diffusion Models</h1>
<!--   <h2 align="center">ICML 2024</h2> -->
  


[Xinghui Li](https://github.com/Crayon-Shinchan), [Qichao Sun](https://github.com/sun631998316), [Pengze Zhang](https://github.com/PangzeCheung), [Fulong Ye](https://scholar.google.com/citations?user=-BbQ5VgAAAAJ&hl=en&oi=ao), [Zhichao Liao](https://lzc-sg.github.io/), [Wanquan Feng](https://scholar.google.com/citations?hl=zh-CN&user=na2akZYAAAAJ&view_op=list_works&sortby=pubdate)✉, [Songtao Zhao](https://crayon-shinchan.github.io/AnyDressing.github.io/)✉, [Qian He](https://scholar.google.com/citations?view_op=list_works&hl=zh-CN&authuser=1&user=9rWWCgUAAAAJ) <br />


### [[`Project Page`](https://crayon-shinchan.github.io/AnyDressing/)][[`arxiv`](https://arxiv.org/abs/2412.04146)][[`Paper`](https://arxiv.org/pdf/2412.04146)]
</div>


## 📃 Abstract
Recent advances in garment-centric image generation from text and image prompts based on diffusion models are impressive. However, existing methods lack support for various combinations of attire, and struggle to preserve the garment details while maintaining faithfulness to the text prompts, limiting their performance across diverse scenarios. 
In this paper, we focus on a new task, i.e., <b><i>Multi-Garment Virtual Dressing</i></b>, and we propose a novel <b>AnyDressing</b> method for customizing characters conditioned on any combination of garments and any personalized text prompts. 
AnyDressing comprises two primary networks named GarmentsNet and DressingNet, which are respectively dedicated to extracting detailed clothing features and generating customized images.
Specifically, we propose an efficient and scalable module called Garment-Specific Feature Extractor in GarmentsNet to individually encode garment textures in parallel. This design prevents garment confusion while ensuring network efficiency. 
Meanwhile, we design an adaptive Dressing-Attention mechanism and a novel Instance-Level Garment Localization Learning strategy in DressingNet to accurately inject multi-garment features into their corresponding regions. This approach efficiently integrates multi-garment texture cues into generated images and further enhances text-image consistency. 
Additionally, we introduce a Garment-Enhanced Texture Learning strategy to improve the fine-grained texture details of garments. 
Thanks to our well-craft design, AnyDressing can serve as a plug-in module to easily integrate with any community control extensions for diffusion models, improving the diversity and controllability of synthesized images. 
Extensive experiments show that AnyDressing achieves state-of-the-art results. 

## 🧭 Overview
<p align="center">
<img src="./static/images/overview.png" width=100% height=100% 
class="center">
</p>

Given <i>N</i> target garments, AnyDressing customizes a character dressed in multiple target garments. 
The GarmentsNet leverages the <b>Garment-Specific Feature Extractor (GFE)</b> module to extract detailed features from multiple garments. 
The DressingNet integrates these features for virtual dressing using a <b>Dressing-Attention (DA)</b> module and an <b>Instance-Level Garment Localization Learning</b> mechanism. 
Moreover, <b>Garment-Enhanced Texture Learning (GTL)</b> strategy further enhances details. 

## 🎨 Updates
  - 🔥 **`2025/02/27`**: Our [**AnyDressing paper**](https://arxiv.org/abs/2412.04146) is accepted by <b>CVPR 2025</b>.
  - **`2024/12/06`**: Our [**AnyDressing paper**](https://arxiv.org/abs/2412.04146) is available.

## 🌏 Code Release
Thank you all for your attention. We are actively cleaning our code and will open source the inference code soon.


    
## 🖊 Citation
If you find AnyDressing useful for your research, welcome to 🌟 this repo and cite our work using the following BibTeX:

```
@article{li2024anydressing,
        title={AnyDressing: Customizable Multi-Garment Virtual Dressing via Latent Diffusion Models},
        author={Xinghui Li and Qi Chao Sun and Pengze Zhang and Fulong Ye and Zhichao Liao and Wanquan Feng and Songtao Zhao and Qian He},
        journal={arXiv preprint arXiv:2412.04146},
        year={2024}
}
```
