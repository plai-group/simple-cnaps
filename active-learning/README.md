# Towards Better Few-Shot Object Recognition - Active Learning

This directory contains the code for the active learning experiments referenced in the paper, "Towards Better Few-Shot Object Recognition", which is currently under review the IEEE TPAMI Special Issue on Learning with Fewer Labels in Computer Vision 2022. We will release a PDF copy of this paper by mid-October.

We would like to also add that this code builds on code developed by Dr. John Bronskill, Jonathan Gordon, James Reqeima, Dr. Sebastian Nowozin, and Dr. Richard E. Turner and kindly shared by Dr. Jogn Bronskil privately. As of writing, they have not publicly released their code for their active learning experiments. If you find the active learning code released here useful, we kingly ask that you also cite their relevant papers as noted in https://github.com/cambridge-mlg/cnaps. Our work was both inspired from their first proposal of "out of the box" few-shot classifiers for active learning and was made possible thanks in part to the code shared with us early in our work.

## Dependencies
You can use the requirements.txt file included to install dependencies for both Simple CNAPS, Transductive CNAPS, relevant active/continual learning experiments and the accompanying source codes for Meta-Dataset, mini-ImageNet and tiered-ImageNet. To install all dependencies, run pip install -r requirements.txt. In general, this code base requires Python 3.5 or greater, PyTorch 1.0 or greater and TensorFlow 2.0 or greater.

## GPU Requirements
We conducted our experiments on two Tesla P100 GPUs with about 10GB of memory each. Lower capacity GPUs can be used to run these experiments by using a lower batch size and modifying parts of the code, as long as the pre-trained checkpoints for Simple and Transductive CNAPS can fit on the GPU(s).

## Dataset Installation
We run active learning experiments on the OMNIGLOT and CIFAR10 benchmarks. For CIFAR10, the code to download the dataset has already been incorporated and the dataset will be setup during the first run. For OMNIGLOT, however, you will need to download the evaluation split of the OMNIGLOT dataset from https://github.com/brendenlake/omniglot/raw/master/python/images_evaluation.zip, unzip and place all images inside an ```omniglot/test``` test folder inside your dataset folder. If you encounter any dataset issues, please make sure that the data paths defined within the load functions for each dataset in ```run_continual_learning.py``` are constructed. Depending on your setup, python is some times unable to create all directories needed.

## Running Active Learning Experiments

All relavant test scripts used to produce the results reported in the paper have been added under the [test-scripts](github.com/plai-group/simple-cnaps/active-learning/test-scripts/) folder in this directory. In general, to run an active learning experiment, please run the following command.

```
python3 run_active_learning.py \
        --data_path <path to datasets, omniglot and cifar10> \
        --feature_adaptation <set to "film" but if your model uses a different strategy for adaptation, specify here> \
        --checkpoint_dir <path to checkpoint directory> \
        --model <specify model, one of simple_cnaps or transductive_cnaps> \
        --dataset <specify dataset name, one of omniglot or cifar 10> 
        --test_model_path <path to trained model checkpoint> \
        --active_learning_method <active learning method to employ>
```

## Citation
We hope you have found our code base helpful! If you use this repository, please cite our papers:

```
@InProceedings{Bateni2020_SimpleCNAPS,
author = {Bateni, Peyman and Goyal, Raghav and Masrani, Vaden and Wood, Frank and Sigal, Leonid},
title = {Improved Few-Shot Visual Classification},
booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2020}
}

@article{Bateni2020_TransductiveCNAPS,
  author    = {Peyman Bateni and Jarred Barber and Jan{-}Willem van de Meent and Frank Wood},
  title     = {Improving Few-Shot Visual Classification with Unlabelled Examples},
  journal   = {CoRR},
  volume    = {abs/2006.12245},
  year      = {2020},
  url       = {https://arxiv.org/abs/2006.12245},
  eprinttype = {arXiv},
  eprint    = {2006.12245},
  timestamp = {Tue, 23 Jun 2020 17:57:22 +0200},
  biburl    = {https://dblp.org/rec/journals/corr/abs-2006-12245.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

@article{Bateni2021_TPAMI_SI_FewShot,
  author    = {Peyman Bateni and Jarred Barber and Raghav Goyal and Vaden Masrani and Jan{-}Willem van de Meent and Leonid Sigal and Frank Wood},
  title     = {Towards Better Few-Shot Object Recognition},
  year      = {2021}
}
```
