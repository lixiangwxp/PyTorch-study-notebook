该文件夹记录了演示使用的notebook，包括以下内容：
- 第零章 前置知识补充
- 第一章 PyTorch的简介和安装（由 `source/` 正文整理的教学练习版）
- 第二章 PyTorch基础知识
- 第三章 PyTorch的主要组成模块（由 `source/` 正文整理的教学练习版）
- 第四章 PyTorch基础实战
  - 图像分类
    - fashion-mnist分类实战
    - 果蔬分类实战
- 第五章 PyTorch模型定义（由 `source/` 正文整理的教学练习版）
- 第六章 PyTorch进阶训练技巧
- 第七章 PyTorch可视化（由 `source/` 正文整理的教学练习版）
- 第八章 PyTorch生态简介
- 第九章 PyTorch的模型部署（由 `source/` 正文整理的教学练习版）
- 第十章 常见网络代码的解读

后续演示代码均会添加进来

## 本地运行环境

本仓库已配置独立的 conda 环境文件 `environment.yml`，推荐使用下面的方式重建环境：

```shell
# 在仓库根目录运行
conda env create -f environment.yml
conda activate pytorch-study-notebook
python -m ipykernel install --user --name pytorch-study-notebook --display-name "PyTorch Study Notebook"
jupyter lab
```

打开 notebook 后，选择 `PyTorch Study Notebook` 内核即可运行。环境中已包含 PyTorch、torchvision、torchtext、timm、imgaug、visdom 和常用 Jupyter 依赖；其中 `numpy<2` 与 `opencv-python<4.12` 是为了兼容旧版 `imgaug`。
