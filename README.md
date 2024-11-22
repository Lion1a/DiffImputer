# DiffImputer

This is the code for paper:
> DiffImputer: Multivariate Dependency-aware Diffusion Network for Spatiotemporal Imputation

## Dependencies
Recent versions of the following packages for Python 3 are required:
* numpy==1.24.1
* PyYAML==6.0.1
* Requests==2.31.0
* scikit_learn==1.5.0
* scipy==1.13.1
* setuptools==69.5.1
* tensorboardX==2.6.2
* torch==1.13.1
* torch_cluster==1.6.0
* torch_geometric==2.5.3
* torch_sparse==0.6.15
* tqdm==4.66.4

## Datasets
All of the datasets we use are publicly available datasets.
### Link
The used datasets are available at:
* Retail_Rocket https://tianchi.aliyun.com/competition/entrance/231719/information/
* Alibaba https://github.com/xuehansheng/DualHGCN
* Amazon https://github.com/YingtongDou/CARE-GNN/tree/master/data
* YelpChi https://docs.dgl.ai/api/python/dgl.data.html#fraud-dataset

Kindly note that there may be two versions of node features for YelpChi. The old version has a dimension of 100 and the new version is 32. In our paper, the results are reported based on the new features.

## Usage
Use the following command to run the main script with configuration options:

* `python main.py --use_cfg --seeds 0 --dataset $dataset`
