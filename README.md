# Improved Few-Shot Visual Classification

This repository contains relevant sources code for the following papers:
- [Improved Few-Shot Visual Classification](https://openaccess.thecvf.com/content_CVPR_2020/html/Bateni_Improved_Few-Shot_Visual_Classification_CVPR_2020_paper.html) @ IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2020
- [Enhancing Few-Shot Image Classification with Unlabelled Examples](https://arxiv.org/abs/2006.12245), IEEE/CVF Winter Conference on Applications of Computer Vision (WACV), 2022 (in submission)
- Towards Better Few-Shot Object Recognition, TPAMI Special Issue on Learning with Fewer Labels in Computer Vision, 2022 (in submission)

The code base has been authored by Peyman Bateni, Jarred Barber, Raghav Goyal, Vaden Masrani, Dr. Jan-Willemn van de Meent, Dr. Leonid Sigal and Dr. Frank Wood. The source code builds upon the original code base for CNAPS authored by John Bronskill, Jonathan Gordon, James Reqeima, Sebastian Nowozin, and Richard E. Turner. We would like to thank them for their help, support and early sharing of their work. To see the original CNAPS repository, visit https://github.com/cambridge-mlg/cnaps.

## Simple CNAPS

Simple CNAPS proposes the use of hierarchically regularized cluster means and covariance estimates within a Mahalanobis-distance based classifer for improved few-shot classification accuracy. This method incorporates said classifier within the same neural adaptive feature extractor as CNAPS. For more details, please refer to our paper on Simple CNAPS: [Improved Few-Shot Visual Classification](https://openaccess.thecvf.com/content_CVPR_2020/html/Bateni_Improved_Few-Shot_Visual_Classification_CVPR_2020_paper.html). The source code for this paper has been provided in the [simple-cnaps-src]() directory. To reproduce our results, please refer to the README.md file within that folder.

Global Meta-Dataset Rank (Simple CNAPS): https://github.com/google-research/meta-dataset#training-on-all-datasets

Global Mini-ImageNet Rank (Simple CNAPS):

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-mini-2)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-2?p=improved-few-shot-visual-classification)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-mini-3)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-3?p=improved-few-shot-visual-classification)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-mini-12)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-12?p=improved-few-shot-visual-classification)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-mini-13)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-13?p=improved-few-shot-visual-classification)

Global Tiered-ImageNet Rank (Simple CNAPS):

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-tiered)](https://paperswithcode.com/sota/few-shot-image-classification-on-tiered?p=improved-few-shot-visual-classification)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-tiered-1)](https://paperswithcode.com/sota/few-shot-image-classification-on-tiered-1?p=improved-few-shot-visual-classification)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-tiered-2)](https://paperswithcode.com/sota/few-shot-image-classification-on-tiered-2?p=improved-few-shot-visual-classification)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improved-few-shot-visual-classification/few-shot-image-classification-on-tiered-3)](https://paperswithcode.com/sota/few-shot-image-classification-on-tiered-3?p=improved-few-shot-visual-classification)

## Transductive CNAPS
Transductive CNAPS extends the Simple CNAPS framework to the transductive few-shot learning setting where all query examples are provided at once. This method uses a two-step transductive task-encoder for adapting the feature extractor as well as a soft k-mean cluster refinement procedure, resulting in better test-time accuracy. For additional details, please refer to our paper on Transductive CNAPS: [Enhancing Few-Shot Image Classification with Unlabelled Examples](https://arxiv.org/abs/2006.12245). The source code for this is provided under the [transductive-cnaps-src]() directory. To reproduce our results, please refer to the README.md file within this folder.

Global Meta-Dataset Rank (Transductive CNAPS): https://github.com/google-research/meta-dataset#training-on-all-datasets

Global Mini-ImageNet Rank (Transductive CNAPS):
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-mini-2)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-2?p=improving-few-shot-visual-classification-with)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-mini-3)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-3?p=improving-few-shot-visual-classification-with)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-mini-12)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-12?p=improving-few-shot-visual-classification-with)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-mini-13)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-13?p=improving-few-shot-visual-classification-with)

Global Tiered-ImageNet Rank (Transductive CNAPS):
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-tiered)](https://paperswithcode.com/sota/few-shot-image-classification-on-tiered?p=improving-few-shot-visual-classification-with)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-tiered-1)](https://paperswithcode.com/sota/few-shot-image-classification-on-tiered-1?p=improving-few-shot-visual-classification-with)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-mini-12)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-12?p=improving-few-shot-visual-classification-with)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/improving-few-shot-visual-classification-with/few-shot-image-classification-on-mini-13)](https://paperswithcode.com/sota/few-shot-image-classification-on-mini-13?p=improving-few-shot-visual-classification-with)

## Dependencies
You can use the ```requirements.txt``` file included to install dependencies for both Simple CNAPS, Transductive CNAPS, relevant active/continual learning experiments and the accompanying source codes for Meta-Dataset, mini-ImageNet and tiered-ImageNet. To install all dependencies, run ```pip install -r requirements.txt```. In general, this code base requires Python 3.5 or greater, PyTorch 1.0 or greater and TensorFlow 2.0 or greater.

## GPU Requirements
The GPU requirements for Simple CNAPS are:
* 1 GPU with 16GB or more memory for training Simple and Transductive CNAPS - you can also perform distributed training of Simple and Transductive CNAPS across 2 GPUs with 8GB or more in dedicated memory
* GPUs with 16GB or more memory for training Simple AR-CNAPS (and Transductive AR-CNAPS should you be interested)
We recommend the same settings for testing.

## Meta-Dataset Results

**Models trained on all datasets (with ```--shuffle_dataset False```)**

| Dataset                         | Simple CNAPS | Simple CNAPS | Transductive CNAPS | Transductive CNAPS |
| ```--shuffle_dataset False```   | False        | True         | False              | True               |
| ---                             | ---          | ---          | ---                | ---                |
| In-Domain Datasets              | ---          | ---          | ---                | ---                |
| ILSVRC                          | 58.6±1.1     | 56.5±1.1     | 58.8±1.1           | 57.9±1.1           |
| Omniglot                        | 91.7±0.6     | 91.9±0.6     | 93.9±0.4           | 94.3±0.4           |
| Aircraft                        | 82.4±0.7     | 83.8±0.6     | 84.1±0.6           | 84.7±0.5           |
| Birds                           | 74.9±0.8     | 76.1±0.9     | 76.8±0.8           | 78.8±0.7           |
| Textures                        | 67.8±0.8     | 70.0±0.8     | 69.0±0.8           | 66.2±0.8           |
| Quick Draw                      | 77.7±0.7     | 78.3±0.7     | 78.6±0.7           | 77.9±0.6           |
| Fungi                           | 46.9±1.0     | 49.1±1.2     | 48.8±1.1           | 48.9±1.2           |
| VGG Flower                      | 90.7±0.5     | 91.3±0.6     | 91.6±0.4           | 92.3±0.4           |
| Out-of-Domain Datasets          | ---          | ---          | ---                | ---                |
| Traffic Signs                   | 73.5±0.7     | 59.2±1.0     | 76.1±0.7           | 59.7±1.1           |
| MSCOCO                          | 46.2±1.1     | 42.4±1.1     | 48.7±1.0           | 42.5±1.1           |
| MNIST                           | 93.9±0.4     | 94.3±0.4     | 95.7±0.3           | 94.7±0.3           |
| CIFAR10                         | 74.3±0.7     | 72.0±0.8     | 75.7±0.7           | 73.6±0.7           |
| CIFAR100                        | 60.5±1.0     | 60.9±1.1     | 62.9±1.0           | 61.8±1.0           |
| ---                             | ---          | ---          | ---                | ---                |
| In-Domain Average Accuracy      | 73.8±0.8     | 74.6±0.8     | 75.2±0.8           | 75.1±0.8           |
| Out-of-Domain Average Accuracy  | 69.7±0.8     | 65.8±0.8     | 71.8±0.8           | 66.5±0.8           |
| Overall Average Accuracy        | 72.2±0.8     | 71.2±0.8     | 73.9±0.8           | 71.8±0.8           |

**Mini-ImageNet Results

| Setup                           | 5-way 1-shot | 5-way 5-shot    | 10-way 1-shot    | 10-way 5-shot    |
| ---                             | ---          | ---             | ---              | ---              |
| Simple CNAPS                    | 53.2±0.9     | 70.8±0.7        | 37.1±0.5         | 56.7±0.5         |
| Simple CNAPS                    | 53.2±0.9     | 70.8±0.7        | 37.1±0.5         | 56.7±0.5         |
| ---                             | ---          | ---             | ---              | ---              |
| Simple CNAPS + FETI             | 77.4±0.8     | 90.3±0.4        | 63.5±0.6         | 83.1±0.4         |
| Simple CNAPS + FETI             | 77.4±0.8     | 90.3±0.4        | 63.5±0.6         | 83.1±0.4         |

**Tiered-ImageNet Results

| Setup                           | 5-way 1-shot | 5-way 5-shot    | 10-way 1-shot    | 10-way 5-shot    |
| ---                             | ---          | ---             | ---              | ---              |
| Simple CNAPS                    | 63.0±1.0     | 80.0±0.8        | 48.1±0.7         | 70.2±0.6         |
| Simple CNAPS                    | 63.0±1.0     | 80.0±0.8        | 48.1±0.7         | 70.2±0.6         |
| ---                             | ---          | ---             | ---              | ---              |
| Simple CNAPS + FETI             | 71.4±1.0     | 86.0±0.6        | 57.1±0.7         | 78.5±0.5         |
| Simple CNAPS + FETI             | 71.4±1.0     | 86.0±0.6        | 57.1±0.7         | 78.5±0.5         |

**Models trained on all datasets (with ```--shuffle_dataset True```)**

| Dataset                         | Simple CNAPS | CNAPS         | 
| ---                             | ---          | ---           |
| In-Domain Datasets              | ---          | ---           |
| ILSVRC                          | 56.5±1.1     | 50.8±1.1      | 
| Omniglot                        | 91.9±0.6     | 91.7±0.5      | 
| Aircraft                        | 83.8±0.6     | 83.7±0.6      | 
| Birds                           | 76.1±0.9     | 73.6±0.9      | 
| Textures                        | 70.0±0.8     | 59.5±0.7      | 
| Quick Draw                      | 78.3±0.7     | 74.7±0.8      | 
| Fungi                           | 49.1±1.2     | 50.2±1.1      | 
| VGG Flower                      | 91.3±0.6     | 88.9±0.5      | 
| Out-of-Domain Datasets          | ---          | ---           |
| Traffic Signs                   | 59.2±1.0     | 56.5±1.1      |
| MSCOCO                          | 42.4±1.1     | 39.4±1.0      |
| MNIST                           | 94.3±0.4     | N/A           |
| CIFAR10                         | 72.0±0.8     | N/A           |
| CIFAR100                        | 60.9±1.1     | N/A           |
| ---                             | ---          | ---           |
| In-Domain Average Accuracy      | 74.6±0.8     | 71.6±0.8      |
| Out-of-Domain Average Accuracy  | 65.8±0.9     | 47.9±1.1*     |
| Overall Average Accuracy        | 71.2±0.8     | 66.9±0.9*     |

```*``` CNAPS averages don't include performances on MNIST, CIFAR10 and CIFAR100

## Mini/Tiered ImageNet Installations & Usage
In order to re-create these experiments, you need to:

1. First clone https://github.com/yaoyao-liu/mini-imagenet-tools, the mini-imagenet tools package used for generating tasks, and https://github.com/yaoyao-liu/tiered-imagenet-tools, the respective tiered-imagenet tools package under ```/src```. Although theoretically this should sufficient, there may be errors arising from hard coded file paths (3 to 4 of which was present at the time of creating our set-up, although they seem to have been resolved since) which you can easily fix.

2. Once the setup is complete, use ```run_simple_cnaps_mt.py``` to run mini\tiered-imagenet experiments:

For Simple CNAPS:
    
    ```cd src; python run_simple_cnaps_mt.py --dataset <choose either mini or tiered> --feature_adaptation film --checkpoint_dir <address of the directory where you want to save the checkpoints> --pretrained_resnet_path <choose resnet pretrained checkpoint>```
    
For Simple AR-CNAPS:
    
    ```cd src; python run_simple_cnaps_mt.py --dataset <choose either mini or tiered> --feature_adaptation film+ar --checkpoint_dir <address of the directory where you want to save the checkpoints> --pretrained_resnet_path <choose resnet pretrained checkpoint>```
    
**Note that as we emphasized this in the main paper, CNAPS-based models including Simple CNAPS have a natural advantage on these benchmarks due to the pre-trianing of the feature extractor on the Meta-Dataset split of ImageNet. We alliviate this issue by re-training the ResNet feature extractor on the specific training splits of mini-ImageNet and tiered-ImageNet. These checkpoints have been provided under ```model-checkpoints/pretrained_resnets``` and are respectively ```pretrained_resnet_mini_imagenet.pt.tar``` and ```
pretrained_resnet_tiered_imagenet.pt.tar```. We additionally consider the case that additional non-test-set overlapping ImageNet classes are used to train our ResNet feature extractor in ```pretrained_resnet_mini_tiered_with_extra_classes.pt.tar```. We refer to this latter setup as "Feature Exctractor Trained (partially) on ImageNet", abbreviated as "FETI". Please visit the experimental section of http://128.84.4.27/abs/2006.12245 for additional details on this setup.

**Updated results (with the new ResNet18 checkpoints - see explanation above) on mini-ImageNet**

| Setup                           | 5-way 1-shot | 5-way 5-shot    | 10-way 1-shot    | 10-way 5-shot    |
| ---                             | ---          | ---             | ---       | ---       |
| Simple CNAPS                    | 53.2±0.9     | 70.8±0.7        | 37.1±0.5  | 56.7±0.5  |
| Simple CNAPS + FETI             | 77.4±0.8     | 90.3±0.4        | 63.5±0.6  | 83.1±0.4  |

**Updated results (with the new ResNet18 checkpoints - see explanation above) on tiered-ImageNet**

| Setup                           | 5-way 1-shot | 5-way 5-shot    | 10-way 1-shot    | 10-way 5-shot    |
| ---                             | ---          | ---             | ---       | ---       |
| Simple CNAPS                    | 63.0±1.0     | 80.0±0.8        | 48.1±0.7  | 70.2±0.6  |
| Simple CNAPS + FETI             | 71.4±1.0     | 86.0±0.6        | 57.1±0.7  | 78.5±0.5  |

## Method Clarification - Use of 1/2 Coefficient on the Mahalanobis Distance

The 1/2 coefficient used in Equation 2, namely the one-half squared Mahalanobis distance, provides correpondence to Gaussian Mixutre Models, but is widely believed to be of little significance as it corresponds to scaling vectors by a factor of 2. This scaling is naturally possible through a feature extractor and it was believed to not have a significant impact on the performance of the model. However, as we observed post-publication, it has a very small but nevertheless noticable impact as the use of the identity matrix in our regularization scheme breaks the equivalency previously believed. To this end, we provided a comparison in performance with respect to the presence of the 1/2 coefficient, and have updated the code to NOT use the coefficient as better performance is observed there. As shown, although overall performance changes are statistically insignificant, on certain specific datasets such as ILSVRC and VGG Flower, the difference is noticable. Note that this effect is primarily significant during training and at test time, either configuration achieves the same performance when used with the same checkpoints. The results shown below were generated with ```--shuffle_dataset False```.

| Dataset                         | Simple CNAPS (without 1/2) | Simple CNAPS (with 1/2)  |
| ---                             | ---                        | ---                      |
| In-Domain Datasets              | ---                        | ---                      |
| ILSVRC                          | 58.6±1.1                   | 55.3±1.1                 |
| Omniglot                        | 91.7±0.6                   | 90.7±0.6                 |
| Aircraft                        | 82.4±0.7                   | 82.0±0.7                 |
| Birds                           | 74.9±0.8                   | 74.2±0.9                 |
| Textures                        | 67.8±0.8                   | 66.0±0.8                 |
| Quick Draw                      | 77.7±0.7                   | 76.3±0.8                 |
| Fungi                           | 46.9±1.0                   | 47.3±1.0                 |
| VGG Flower                      | 90.7±0.5                   | 87.9±0.6                 |
| Out-of-Domain Datasets          | ---                        | ---                      |
| Traffic Signs                   | 73.5±0.7                   | 74.7±0.7                 |
| MSCOCO                          | 46.2±1.1                   | 47.4±1.1                 |
| MNIST                           | 93.9±0.4                   | 94.3±0.4                 |
| CIFAR10                         | 74.3±0.7                   | 72.0±0.8                 |
| CIFAR100                        | 60.5±1.0                   | 58.7±1.0                 |
| ---                             | ---                        | ---                      |
| In-Domain Average Accuracy      | 73.8±0.8                   | 72.5±0.8                 |
| Out-of-Domain Average Accuracy  | 69.7±0.8                   | 69.4±0.8                 |
| Overall Average Accuracy        | 72.2±0.8                   | 71.3±0.8                 |

## Citing this repository/paper
```
@InProceedings{Bateni_2020_CVPR,
author = {Bateni, Peyman and Goyal, Raghav and Masrani, Vaden and Wood, Frank and Sigal, Leonid},
title = {Improved Few-Shot Visual Classification},
booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2020}
}
```
