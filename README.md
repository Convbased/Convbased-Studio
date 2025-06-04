# Convbased-Studio

<div align="center">

[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Models-yellow?style=for-the-badge)](https://huggingface.co/PluginsKers/Convbased-Studio)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.3.1-red?style=for-the-badge&logo=pytorch)](https://pytorch.org/)

</div>

## 项目简介

本项目专注于训练高质量的RVC（Retrieval-based Voice Conversion）模型底模，为语音转换任务提供强大的基础模型支持。通过476个不同说话人的多样化数据集，我们训练出了具有优异收敛性能的编码器和解码器模型。

## ✨ 主要特性

- **大规模多说话人训练**: 基于476个说话人的丰富数据集
- **优异的收敛性能**: 经过35天深度训练，提供更稳定的训练收敛能力
- **高质量编码器/解码器**: 为RVC模型训练提供强大的预训练底模
- **完整的训练流程**: 包含数据预处理、模型训练、评估等完整工具链

## 🎯 模型特点

### 训练规模
- **说话人数量**: 476个不同说话人
- **训练时长**: 35天连续训练
- **模型类型**: 编码器 + 解码器架构

### 性能优势
- 更快的训练收敛速度
- 更稳定的训练过程
- 更好的语音质量输出

## 📥 模型下载

### 预训练模型下载

| 声码器 | 32k | 40k | 48k |
|:---:|:---:|:---:|:---:|
| **HiFi-GAN MRF** | 🚧 即将发布 | 🚧 即将发布 | 🚧 即将发布 |
| **HiFi-GAN NSF** | 🚧 即将发布 | 🚧 即将发布 | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio) |
| **HiFi-GAN** | 🚧 即将发布 | 🚧 即将发布 | 🚧 即将发布 |
| **RefineGAN** | 🚧 即将发布 | 🚧 即将发布 | 🚧 即将发布 |

> 💡 **使用建议**: 推荐使用 HiFi-GAN NSF 48k 模型，具有最佳的音质表现和训练稳定性。


### 训练数据集

本模型使用以下高质量中文语音数据集进行训练：

| 数据集名称         | 时长（小时） | 描述 |
|-------------------|-------------|------|
| data_aishell      | 178         | 中文普通话语音识别数据集 |
| data_thchs30      | 30          | 清华大学中文语音数据集 |
| primewords_md_2018| 178         | 中文语音合成数据集 |
| VCTK              | 44          | 英文多说话人数据集 |
| 四川方言           | 4          | 四川话方言数据 |
| 闽南语             | 3          | 闽南话方言数据 |
| 粤语              | 3           | 粤语方言数据 |
| 温州方言           | 7          | 温州话方言数据 |
| 噪声              | 20          | 噪声环境语音数据 |

## 🚀 快速开始

### 环境要求
- Python 3.11+
- CUDA 11.0+ (推荐使用GPU训练)
- 8GB+ GPU显存 (推荐16GB+)

### 依赖安装
```bash
# 安装项目依赖
pip install -r requirements.txt

# 或使用安装脚本
./run-install.sh
```

### 数据处理

具体查看 `data_preprocessing.ipynb`

### 模型训练

具体查看 `train.ipynb`

## 🛠️ 使用说明

### 配置文件

底模 convbased_v1 使用目前只有48k采样率

## 🙏 致谢

感谢 [Applio](https://github.com/IAHispano/Applio) 项目为语音转换领域做出的卓越贡献。Applio作为一个强大的语音转换工具，专注于简单性、质量和性能，为我们的研究和开发提供了重要的参考和启发。


感谢 [Convbased](https://weights.chat/) 为本项目提供计算服务，Convbased 致力于推进中文语音合成技术与云计算的发展。

## 📄 许可证

本项目采用 Apache License 2.0 许可证，详见 [LICENSE](LICENSE) 文件。

## 🤝 贡献

欢迎提交Issues和Pull Requests来帮助改进项目！

## 📧 联系方式

如有问题或建议，请通过以下方式联系：
- 提交GitHub Issue
- 发送邮件至项目维护者

---

*本模型致力于推进中文语音合成技术的发展，该底模已用于微调大部分模型于 [Convbased](https://weights.chat/)*