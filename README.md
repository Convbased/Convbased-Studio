# Convbased-Studio

<div align="center">

[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Models-yellow?style=for-the-badge)](https://huggingface.co/PluginsKers/Convbased-Studio)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.3.1-red?style=for-the-badge&logo=pytorch)](https://pytorch.org/)

</div>

## 项目简介

本项目专注于训练高质量的预训练底模，为语音转换任务提供强大的基础模型支持。


| 特征提取 | 声码器 | 40k | 48k |
|-----------|--------|-----|-----|
| contentvec | hifigannsf | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio) |
| contentvec | sifigan | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio) |
| contentvec | refinegan | ❌ | ❌ |
| contentvec | hifiganmrf | ❌ | ❌ |
| spin | hifigannsf | ❌ | ❌ |
| spin | sifigan | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio) |
| spin | refinegan | ❌ | ❌ |
| spin | hifiganmrf | ❌ | ❌ |
| chinese-hubert-base | hifigannsf | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio) |
| chinese-hubert-base | sifigan | ❌ | ❌ |
| chinese-hubert-base | refinegan | ❌ | ❌ |
| chinese-hubert-base | hifiganmrf | ❌ | ❌ |

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

## 🙏 致谢

感谢 [RVC](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) 项目为语音转换领域做出的卓越贡献。


感谢 [Convbased](https://weights.chat/) 为本项目提供计算服务，Convbased 致力于推进中文语音合成技术与云计算的发展。

## 📄 许可证

本项目采用 MIT 许可证，详见 [LICENSE](LICENSE) 文件。

## 🤝 贡献

欢迎提交Issues和Pull Requests来帮助改进项目！

## 📧 联系方式

如有问题或建议，请通过以下方式联系：
- 提交GitHub Issue
- 发送邮件至项目维护者

---

![dbe327da212afd5f41f819a817e08b68](https://github.com/user-attachments/assets/c6be570b-1ea5-4811-b253-2d993d5f574a)


*致力于推进中文语音合成技术的发展，该底模已用于微调大部分模型于 [Convbased](https://weights.chat/)*
