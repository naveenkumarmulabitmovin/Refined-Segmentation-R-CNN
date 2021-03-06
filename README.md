# Refined Segmentation R-CNN
  
**Accepted by MICCAI2019.**  

Liu, Yalong, Jie Li, Ying Wang, Miaomiao Wang, Xianjun Li, Zhicheng Jiao, Jian Yang, and Xingbo Gao. "Refined Segmentation R-CNN: A Two-Stage Convolutional Neural Network for Punctate White Matter Lesion Segmentation in Preterm Infants." In International Conference on Medical Image Computing and Computer-Assisted Intervention, pp. 193-201. Springer, Cham, 2019.  
![MICCAI2019_logo](./imgs/MICCAI2019_logo.png)  

--A Deep Learning method to segment punctate white matter lesions (PWMLs); Brain tumor segmentation.  

**By:** Yalong Liu<sup>1</sup>, Jie Li<sup>1</sup>, Ying Wang<sup>1</sup>, Miaomiao Wang<sup>2</sup>, Xianjun Li<sup>2</sup>, Zhicheng Jiao<sup>3</sup>, Jian Yang<sup>2</sup>, Xingbo Gao<sup>1</sup>  
1. Lab of Video and Image Processing Systems, School of Electronic Engineering, Xidian University, Xi’an 710071, China  
2. Department of Radiology, The First Affiliated Hospital of Xi'an Jiaotong University, Xi’an 710061, China  
3. University of North Carolina at Chapel Hill, Chapel Hill, NC 27599, USA


**This repository includes:**  
1.T1WI of 10 patients for test(Full dataset is not allowed to be made public; Warning:The provided test data is only used to test the code. Please use your own data to train a normal model.)  
2.Full code for model training and inference   
3.The link of pre-trained weights on google drive   

## Requirements
Python 3.6.3  
Tensorflow-gpu 1.12.0  
CUDA 9.0  
## Getting Started
1.Download the repositories and weights([GoogleDrive](https://drive.google.com/file/d/1EoRhtFphayInBlr9IJmaKXqu8BTt3E7M/view?usp=sharing) or [Anonfiles](https://anonfiles.com/I2xeTaS5m1/model_enhancedrpn_enlargeroi1.3_segnet_crf_pwml_98765_h5) or [BaiduYun](https://pan.baidu.com/s/1rdlAWDasaVt6UF7X_AhRNg)).  
2.Choose a mode in the main.py('inference' or 'training').  
3.(optional)Change parameters in configs.py according to the comment  in the file.  
4.python ./main.py  
Enjoy!

## Acknowledgment
This repo borrows tons of code from  
[matterport/Mask_RCNN](https://github.com/matterport/Mask_RCNN)  
## Results
Performance:  

Index|--------Original MRI--------|---------SOTA----------|-----Mask R-CNN------|-----Our Method--------
:--|:--:|:--:|:--:|:--:


&nbsp;8/77&nbsp;|![8_77](./imgs/8_77.png)
:--|:--:|
&nbsp;79/67&nbsp;|![79_67](./imgs/79_67.png)  
&nbsp;82/67&nbsp;|![82_67](./imgs/82_67.png)  
&nbsp;83/48&nbsp;|![83_48](./imgs/83_48.png)  
&nbsp;83/54&nbsp;|![83_54](./imgs/83_54.png)
&nbsp;83/80&nbsp;|![83_80](./imgs/83_80.png)

-----
### Citation
If you use Refined Segmentation R-CNN in your research, please cite the paper([MICCAI2019-Springer](https://link.springer.com/chapter/10.1007%2F978-3-030-32248-9_22)) or ([Arxiv](http://arxiv.org/abs/1906.09684)):
```
Liu, Yalong, Jie Li, Ying Wang, Miaomiao Wang, Xianjun Li, Zhicheng Jiao, Jian Yang, and Xingbo Gao. "Refined Segmentation R-CNN: A Two-Stage Convolutional Neural Network for Punctate White Matter Lesion Segmentation in Preterm Infants." In International Conference on Medical Image Computing and Computer-Assisted Intervention, pp. 193-201. Springer, Cham, 2019.
```
For  more information about me, please refer to my [personal website](https://yalongliu.github.io/)











