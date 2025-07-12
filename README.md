<img src="/assets/cover.png" width="100%" />
<hr />
<div align="center">

[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Models-yellow?style=for-the-badge)](https://huggingface.co/PluginsKers/Convbased-Studio)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

</div>

## 项目简介

本项目专注于训练高质量的预训练底模，为语音转换任务提供强大的基础模型支持。

| 特征提取 | 声码器 | 采样率40k | 采样率48k |
|-----------|--------|-----|-----|
| contentvec | hifigannsf | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio/tree/main/contentvec/hifigan-nsf/476sid) |
| contentvec | sifigan | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio/tree/main/contentvec/sifigan) |
| spin | hifigannsf | ❌ |  [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio/tree/main/spin/hifigan-nsf) |
| spin | sifigan | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio/tree/main/spin/sifigan) |
| chinese-hubert-base | hifigannsf | ❌ | [![Download](https://img.shields.io/badge/下载-HuggingFace-yellow)](https://huggingface.co/PluginsKers/Convbased-Studio/tree/main/chinese-hubert-base/hifigan-nsf) |
| chinese-hubert-base | sifigan | ❌ | ❌ |

## 许可证

本项目采用 MIT 许可证，详见 [LICENSE](LICENSE) 文件。

## 贡献

欢迎提交Issues和Pull Requests来帮助改进项目！

## 加入交流

<img src="/assets/qrcode.png" width="256px" height="256px" />


*致力于推进中文语音合成技术的发展，该底模已用于微调大部分模型于 [Convbased Studio](https://weights.chat/)*
