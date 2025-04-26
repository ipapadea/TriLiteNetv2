# TriLiteNet





## Requirement

This codebase has been developed with python version 3.8, PyTorch 1.8.0 and torchvision 0.9.0

```setup
pip install -r requirements.txt
```



## Pre-trained Model
You can get the pre-trained model from <a href="https://drive.google.com/drive/folders/1wLZqemCxxzwiFeFUGY1zMaqcKoQLHFyK?usp=sharing">here</a>.


## Dataset
- Download the images from [images](https://bdd-data.berkeley.edu/).
- Download the annotations of detection from [det_annotations](https://drive.google.com/file/d/1Ge-R8NTxG1eqd4zbryFo-1Uonuh0Nxyl/view?usp=sharing). 
- Download the annotations of drivable area segmentation from [da_seg_annotations](https://drive.google.com/file/d/1xy_DhUZRHR8yrZG3OwTQAHhYTnXn7URv/view?usp=sharing). 
- Download the annotations of lane line segmentation from [ll_seg_annotations](https://drive.google.com/file/d/1lDNTPIQj_YLNZVkksKM25CvCHuquJ8AP/view?usp=sharing). 

We recommend the dataset directory structure to be the following:

```
# The id represent the correspondence relation
├─dataset root
│ ├─images
│ │ ├─train
│ │ ├─val
│ ├─det_annotations
│ │ ├─train
│ │ ├─val
│ ├─da_seg_annotations
│ │ ├─train
│ │ ├─val
│ ├─ll_seg_annotations
│ │ ├─train
│ │ ├─val
```

Update the your dataset path in the `lib/config/default.py`.


## Acknowledgements

This work would not have been possible without the valuable contributions of the following authors.


* [YOLOP](https://github.com/hustvl/YOLOP)
* [TwinLiteNet](https://github.com/chequanghuy/TwinLiteNet)
* [TwinLiteNetPlus](https://github.com/chequanghuy/TwinLiteNetPlus)
* [Partial Class Activation Attention for Semantic Segmentation](https://github.com/lsa1997/PCAA)
* [ESPNet](https://github.com/sacmehta/ESPNet)

## Citation

```BibTeX
@article{che2024twinlitenetplus,
      title={TwinLiteNetPlus: A Stronger Model for Real-time Drivable Area and Lane Segmentation}, 
      author={Quang-Huy Che and Duc-Tri Le and Minh-Quan Pham and Vinh-Tiep Nguyen and Duc-Khai Lam},
      year={2024},
      eprint={2403.16958},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2403.16958}, 
}
```

