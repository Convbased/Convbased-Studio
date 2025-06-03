# Convbased-Studio

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
- 适用于多种RVC训练场景

### 支持的声码器
- **HiFi-GAN MRF**: 多感受野HiFi-GAN声码器
- **HiFi-GAN NSF**: 神经源滤波器HiFi-GAN声码器
- **HiFi-GAN**: 经典HiFi-GAN声码器
- **RefineGAN**: 高质量音频生成声码器

## 🚀 快速开始

### 环境要求
- Python 3.8+
- CUDA 11.0+ (推荐使用GPU训练)
- 8GB+ GPU显存 (推荐16GB+)

### 安装依赖
```bash
# 安装项目依赖
pip install -r requirements.txt

# 或使用安装脚本
./run-install.sh
```

### 📔 使用指南

#### 1. 数据预处理

data_preprocessing.ipynb

#### 2. 模型训练

train.ipynb

## 🛠️ 使用说明

### 配置文件

底模 convbased_v1 使用目前只有48k采样率

### GPU配置
系统会自动检测可用GPU并进行优化配置：
- 支持多GPU训练
- 自动内存管理
- 动态批处理大小调整

## 📊 训练监控

使用TensorBoard监控训练过程：
```bash
tensorboard --logdir logs/
```

## 🙏 致谢

感谢 [Applio](https://github.com/IAHispano/Applio) 项目为语音转换领域做出的卓越贡献。Applio作为一个强大的语音转换工具，专注于简单性、质量和性能，为我们的研究和开发提供了重要的参考和启发。


感谢 [Convbased](https://weights.chat/) 为本项目提供计算服务，Convbased 致力于推进中文语音合成技术与云计算的发展。

## 📄 许可证

本项目采用MIT许可证，详见 [LICENSE](LICENSE) 文件。

## 🤝 贡献

欢迎提交Issues和Pull Requests来帮助改进项目！

## 📧 联系方式

如有问题或建议，请通过以下方式联系：
- 提交GitHub Issue
- 发送邮件至项目维护者

---

*本模型致力于推进中文语音合成技术的发展，该底模已用于微调大部分模型于 [Convbased](https://weights.chat/)*