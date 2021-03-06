# CBNet: A Novel Composite Backbone Network Architecture for Object Detection

by Yudong Liu,Yongtao Wang, Siwei Wang, Tingting Liang.

## Introduction

We have released our code at https://github.com/PKUbahuangliuhe/CBNet implemented by caffe2. Since [Detectron](https://github.com/facebookresearch/Detectron) code will not be maintained, we release our implementation based on [mmdetection](https://github.com/open-mmlab/mmdetection)

Please follow [mmdetection](https://github.com/open-mmlab/mmdetection) on how to install the environment.

You need to convert the original backbone to cbnet version with **python convert_db.py** or **python convert_tb.py**.

Our CBNetv2 will be released soon.

Contact us with bahuangliuhe@pku.edu.cn,wyt@pku.edu.cn.

**The project is only free for academic research purposes, but needs authorization for commerce. For commerce permission, please contact wyt@pku.edu.cn.**


## Citation

If you use our code/model/data, please cite our paper:
https://aaai.org/Papers/AAAI/2020GB/AAAI-LiuY.1833.pdf



### Detection results on COCO val2017

|  Baseline |   Backbone   | Input size       | box AP |                 
| :------------------------: | :-------------: | :-----: |:-------: |
|     FPN   |   ResNext-101-32x4d     |  1333x800 | 40.1  |
|     FPN   |   Dual-ResNeXt-101-32x4d  |  1333x800| 41.5  |
|     FPN   |   Triple-ResNeXt-101-32x4d |  1333x800 | 42.0  |
|     FPN   |   Dual-ResNeXt-101-32x4d(**CBNetv2**) |  1333x800 | 43.2  |
|Cascade R-CNN(with DCN and multi-scale training)| Dual-ResNeXt-101-32x4d(**CBNetv2**)|  1333x800|51.2(51.6 on 2017test-dev)  |
