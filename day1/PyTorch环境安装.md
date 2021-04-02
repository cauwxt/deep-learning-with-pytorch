# PyTorch环境安装

## 安装VScode

安装最新版本的VScode: <https://code.visualstudio.com/>

## 安装anaconda

版本：最新

地址：<https://www.python.org/downloads/windows/>

注意事项：添加到Path环境变量

## 安装CUDA工具包

注：电脑支持GPU

版本：11.1

网址：<https://developer.nvidia.com/zh-cn/cuda-downloads?>

## 安装Pytorch

网址：<https://pytorch.org/>

步骤：

- 选择操作系统

- 选择安装方式：conda
  
- 选择编程语言：python

- 选择cuda版本或cpu

```python
conda install pytorch torchvision torchaudio cudatoolkit=11.1 -c pytorch -c conda-forge
```

## 安装Windows Terminal

在Microsoft store中安装

## 建立虚拟环境

- 打开Windows Terminal
- 初始化，输入 `conda init`
- 重启Windows Terminal
- 创建新环境，输入 `conda create --name pytorch python=3.7`
- 安装完成之后激活新环境，`conda activate pytorch`
- 安装PyTorch，输入`conda install pytorch torchvision torchaudio cudatoolkit=11.1 -c pytorch -c conda-forge`
- 安装jupyter notebook，`pip install jupyter notebook -i https://pypi.tuna.tsinghua.edu.cn/simple`
- 验证是否安装完成
  
```python
import torch
print(torch.cuda.is_available())
```
