# 模式识别与应用期末作业

2022年春季学期模式识别与应用课程期末作业：基于Oracle-MNIST数据集的分类实验与探究。

## 实验要求

### 基础要求

* 根据数据集[[数据集链接](https://github.com/wm-bupt/oracle-mnist)]的规定，明确区分训练集和测试集，明确识别性能评价方法。
* 对应大作业题目内容，说明模式识别的基本流程。
* 实验测试至少两种分类算法（分类器），不限课上内容，附参考文献。
* 编程语言不限，可以使用开源代码，但需要标注说明。
* 比较分析实验方法的优劣（原理、实验结果，两个方面要匹配）。

### 加分项

* 对该问题有自己的新想法并实验（清楚表达），或者试验了一个特别新颖的分类方法，结果显示的图表工整清晰。
* 得到的结果与已有的SOTA方法（最新方法，例如近五年）进行理论和实验的比较，并分析优劣。
* 对新数据集的使用和构建提出实质的疑问和建议！

## 环境配置

* Python 3.6.7
* PyTorch 1.0.0

* Keras 2.9.0
* Numpy 1.14.5
* Pandas 1.15
* Scikit-learn 0.24.2

## 分类方法

### 传统机器学习方法



### ResNet18

[[原文]](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)

### ResNet18迁移学习



### Vision Transformer（ViT）

[[原文](https://arxiv.org/pdf/2010.11929.pdf)]

[[我知乎上的笔记](https://zhuanlan.zhihu.com/p/463996775)]

由于ViT打破了计算机视觉与自然语言处理之间的壁垒，因此各路大神在ViT上疯狂内卷，因此当然要用ViT试一试新的数据集（手动狗头）

### VGG5（SpinalNet）





## 文件说明

文件结构如下图所示：



运行代码：

（一）对于机器学习方法：

```python

```

（二）对于ResNet18迁移学习方法：

```python
python3 train_pytorch.py --lr 0.1 --epochs 15 --net MnistResNet --data-dir ../data/oracle/ --use-cuda
```


## 引用

如果你也在进行相关的工作并且本项目的代码可以对你的研究提供帮助，欢迎引用：

使用bibtex：

* 本项目的代码

```latex
@misc{oraclemnisthomework,
   author = {Chen, Wentao},
   title = {Experiments and Explorations on Classification Based on Oracle-MNIST Dataset},
   howpublished = {\url{https://github.com/realmadridchenwentao/Oracle-MNIST}}
}
```

* 数据集论文

```latex
@article{wang2022oracle,
  title={Oracle-MNIST: a Realistic Image Dataset for Benchmarking Machine Learning Algorithms},
  author={Wang, Mei and Deng, Weihong},
  journal={arXiv preprint arXiv:2205.09442},
  pages={1--7},
  year={2022}
}
```


