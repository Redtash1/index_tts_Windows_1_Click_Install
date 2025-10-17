<div align="center">


# DON'T CLONE THIS REPO, IT WON'T WORK AS IT ALL DEPENDS ON THE PYTHON_EMBEDED 3.10.9 TO WORK! 


## I made this Index TTS2 Portable 1 click install for Windows that uses Nvidia GTX 10XX, 16XX, RTX Quadro, 20XX, 30XX, 40XX, 50XX.  During installation it will update Index TTS2, install Torch 2.8.0+CU128. Creates Launch Index TTS2 & Voices Desktop Shortcuts. All Index TTS2 updates comes directly from the original index-tts/index-tts Repository. 

## Click here to jump to Install 👉 [Installation](#-Installation) 👈

# [![Downloads](https://img.shields.io/github/downloads/Redtash1/Wan2GP-Windows-One-Click-Install-With-Sage/total.svg)](https://github.com/Redtash1/Wan2GP-Windows-One-Click-Install-With-Sage/releases)
</div>

<img width="1879" height="879" alt="index_tts" src="https://github.com/user-attachments/assets/05aaaca0-ac2b-4898-af3a-96230bc59b1c" />

</div>
</div>
<div align="center">
<img src='assets/index_icon.png' width="250"/>
</div>

<div align="center">
<a href="docs/README_zh.md" style="font-size: 24px">简体中文</a> | 
<a href="README.md" style="font-size: 24px">English</a>
</div>

## 👉🏻 IndexTTS2 👈🏻

<center><h3>IndexTTS2: A Breakthrough in Emotionally Expressive and Duration-Controlled Auto-Regressive Zero-Shot Text-to-Speech</h3></center>

[![IndexTTS2](assets/IndexTTS2_banner.png)](assets/IndexTTS2_banner.png)


<div align="center">
  <a href='https://arxiv.org/abs/2506.21619'>
    <img src='https://img.shields.io/badge/ArXiv-2506.21619-red?logo=arxiv'/>
  </a>
  <br/>
  <a href='https://github.com/index-tts/index-tts'>
    <img src='https://img.shields.io/badge/GitHub-Code-orange?logo=github'/>
  </a>
  <a href='https://index-tts.github.io/index-tts2.github.io/'>
    <img src='https://img.shields.io/badge/GitHub-Demo-orange?logo=github'/>
  </a>
  <br/>
  <a href='https://huggingface.co/spaces/IndexTeam/IndexTTS-2-Demo'>
    <img src='https://img.shields.io/badge/HuggingFace-Demo-blue?logo=huggingface'/>
  </a>
  <a href='https://huggingface.co/IndexTeam/IndexTTS-2'>
    <img src='https://img.shields.io/badge/HuggingFace-Model-blue?logo=huggingface' />
  </a>
  <br/>
  <a href='https://modelscope.cn/studios/IndexTeam/IndexTTS-2-Demo'>
    <img src='https://img.shields.io/badge/ModelScope-Demo-purple?logo=modelscope'/>
  </>
  <a href='https://modelscope.cn/models/IndexTeam/IndexTTS-2'>
    <img src='https://img.shields.io/badge/ModelScope-Model-purple?logo=modelscope'/>
  </a>
</div>


### Abstract

Existing autoregressive large-scale text-to-speech (TTS) models have advantages in speech naturalness, but their token-by-token generation mechanism makes it difficult to precisely control the duration of synthesized speech. This becomes a significant limitation in applications requiring strict audio-visual synchronization, such as video dubbing.

This paper introduces IndexTTS2, which proposes a novel, general, and autoregressive model-friendly method for speech duration control.

The method supports two generation modes: one explicitly specifies the number of generated tokens to precisely control speech duration; the other freely generates speech in an autoregressive manner without specifying the number of tokens, while faithfully reproducing the prosodic features of the input prompt.

Furthermore, IndexTTS2 achieves disentanglement between emotional expression and speaker identity, enabling independent control over timbre and emotion. In the zero-shot setting, the model can accurately reconstruct the target timbre (from the timbre prompt) while perfectly reproducing the specified emotional tone (from the style prompt).

To enhance speech clarity in highly emotional expressions, we incorporate GPT latent representations and design a novel three-stage training paradigm to improve the stability of the generated speech. Additionally, to lower the barrier for emotional control, we designed a soft instruction mechanism based on text descriptions by fine-tuning Qwen3, effectively guiding the generation of speech with the desired emotional orientation.

Finally, experimental results on multiple datasets show that IndexTTS2 outperforms state-of-the-art zero-shot TTS models in terms of word error rate, speaker similarity, and emotional fidelity. Audio samples are available at: <a href="https://index-tts.github.io/index-tts2.github.io/">IndexTTS2 demo page</a>.

**Tips:** Please contact the authors for more detailed information. For commercial usage and cooperation, please contact <u>indexspeech@bilibili.com</u>.


### Feel IndexTTS2

<div align="center">

**IndexTTS2: The Future of Voice, Now Generating**

[![IndexTTS2 Demo](assets/IndexTTS2-video-pic.png)](https://www.bilibili.com/video/BV136a9zqEk5)

*Click the image to watch the IndexTTS2 introduction video.*

</div>


### Contact

QQ Group：663272642(No.4) 1013410623(No.5)  \
Discord：https://discord.gg/uT32E7KDmy  \
Email：indexspeech@bilibili.com  \
You are welcome to join our community! 🌏  \
欢迎大家来交流讨论！

> [!CAUTION]
> Thank you for your support of the bilibili indextts project!
> Please note that the **only official channel** maintained by the core team is: [https://github.com/index-tts/index-tts](https://github.com/index-tts/index-tts).
> ***Any other websites or services are not official***, and we cannot guarantee their security, accuracy, or timeliness.
> For the latest updates, please always refer to this official repository.


## 📣 Updates

- `2025/09/08` 🔥🔥🔥  We release **IndexTTS-2** to the world!
    - The first autoregressive TTS model with precise synthesis duration control, supporting both controllable and uncontrollable modes. <i>This functionality is not yet enabled in this release.</i>
    - The model achieves highly expressive emotional speech synthesis, with emotion-controllable capabilities enabled through multiple input modalities.
- `2025/05/14` 🔥🔥 We release **IndexTTS-1.5**, significantly improving the model's stability and its performance in the English language.
- `2025/03/25` 🔥 We release **IndexTTS-1.0** with model weights and inference code.
- `2025/02/12` 🔥 We submitted our paper to arXiv, and released our demos and test sets.


## 🖥️ Neural Network Architecture

Architectural overview of IndexTTS2, our state-of-the art speech model:

<picture>
  <img src="assets/IndexTTS2.png"  width="800"/>
</picture>


The key contributions of **IndexTTS2** are summarized as follows:

 - We propose a duration adaptation scheme for autoregressive TTS models. IndexTTS2 is the first autoregressive zero-shot TTS model to combine precise duration control with natural duration generation, and the method is scalable for any autoregressive large-scale TTS model.  
 - The emotional and speaker-related features are decoupled from the prompts, and a feature fusion strategy is designed to maintain semantic fluency and pronunciation clarity during emotionally rich expressions. Furthermore, a tool was developed for emotion control, utilizing natural language descriptions for the benefit of users.  
 - To address the lack of highly expressive speech data, we propose an effective training strategy, significantly enhancing the emotional expressiveness of zeroshot TTS to State-of-the-Art (SOTA) level.  
 - We will publicly release the code and pre-trained weights to facilitate future research and practical applications.  


## Model Download

| **HuggingFace**                                          | **ModelScope** |
|----------------------------------------------------------|----------------------------------------------------------|
| [😁 IndexTTS-2](https://huggingface.co/IndexTeam/IndexTTS-2) | [IndexTTS-2](https://modelscope.cn/models/IndexTeam/IndexTTS-2) |
| [IndexTTS-1.5](https://huggingface.co/IndexTeam/IndexTTS-1.5) | [IndexTTS-1.5](https://modelscope.cn/models/IndexTeam/IndexTTS-1.5) |
| [IndexTTS](https://huggingface.co/IndexTeam/Index-TTS) | [IndexTTS](https://modelscope.cn/models/IndexTeam/Index-TTS) |


# 📦 Installation

## Nvidia GTX 10XX, 16XX, RTX Quadro, 20XX, 30XX, 40XX, 50XX

### All Index TTS updates comes directly from the original index tts/index tts Repository.

1. Make sure you have Git installed as it will be needed to update Index TTS, if not download the Git Standalone Installer and click on Git for Windows/x64 Setup. 👉 [Git Standalone Installer Download](https://git-scm.com/downloads/win) 👈 To install Git, double click Git.exe and just keep clicking next until it's installed, you don't need to change anything.


2. Make sure your Nvidia graphics drivers are up-to-date. If they are not or if your not sure, please click on the following link to download Nvidia graphics drivers. 👉 [Nvidia Drivers](https://www.nvidia.com/en-us/software/nvidia-app/) 👈

3. Make sure that you have NVIDIA's [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) version **12.8** (or newer) installed on your system.

4.  Now after you have made sure Nvidia GPU drivers are up to date and Git is installed, download index_tts.exe from here 👉 [Wan2GP-Windows-One-Click-Install-With-Sage](https://github.com/Redtash1/Wan2GP-Windows-One-Click-Install-With-Sage/releases) 👈 or from the Releases section at the top right of this page.

5. After downloading, double click index_tts.exe and pick where you would like to extract the zip files too.

6. Then open Index TTS main folder and you will see this in the root


<img width="758" height="413" alt="index_tts1" src="https://github.com/user-attachments/assets/5327d633-0e57-450c-8954-766b209d163d" />


</div>

7. Then double click on the Install_Index_TTS.bat to start the installation. After installation is finished, slowly scroll back up to the top to make sure everything installed correctly.

8. To launch Index TTS you can use either the Launch_Index_TTS.bat for normal VRAM or Launch_Index_TTS_LOW_VRAM.bat for Low VRAM in the current folder or the Desktop shortcut but this will Launch Normal VRAM.

### If this worked for you, Please give it a Star ⭐. Thank you.



## Alternative Models download via `modelscope` if 'Huggingface' doesn't work for you.

Use the Download_Models_Via_Modelscope.bat to download from Modelscope, it will automatically download the models into checkpoints folder.




### Have fun!


### 🔥 IndexTTS2 Tips



> [!IMPORTANT]
> It can be very helpful to use Argument --fp16 **FP16** (half-precision) inference. It is faster
> and uses less VRAM, with a very small quality loss.
> 





For more detailed information, see [README_INDEXTTS_1_5](archive/README_INDEXTTS_1_5.md),
or visit the IndexTTS1 repository at <a href="https://github.com/index-tts/index-tts/tree/v1.5.0">index-tts:v1.5.0</a>.


## Our Releases and Demos

### IndexTTS2: [[Paper]](https://arxiv.org/abs/2506.21619); [[Demo]](https://index-tts.github.io/index-tts2.github.io/); [[ModelScope]](https://modelscope.cn/studios/IndexTeam/IndexTTS-2-Demo); [[HuggingFace]](https://huggingface.co/spaces/IndexTeam/IndexTTS-2-Demo)

### IndexTTS1: [[Paper]](https://arxiv.org/abs/2502.05512); [[Demo]](https://index-tts.github.io/); [[ModelScope]](https://modelscope.cn/studios/IndexTeam/IndexTTS-Demo); [[HuggingFace]](https://huggingface.co/spaces/IndexTeam/IndexTTS)


## Acknowledgements

1. [tortoise-tts](https://github.com/neonbjb/tortoise-tts)
2. [XTTSv2](https://github.com/coqui-ai/TTS)
3. [BigVGAN](https://github.com/NVIDIA/BigVGAN)
4. [wenet](https://github.com/wenet-e2e/wenet/tree/main)
5. [icefall](https://github.com/k2-fsa/icefall)
6. [maskgct](https://github.com/open-mmlab/Amphion/tree/main/models/tts/maskgct)
7. [seed-vc](https://github.com/Plachtaa/seed-vc)

## Contributors in Bilibili
We sincerely thank colleagues from different roles at Bilibili, whose combined efforts made the IndexTTS series possible.

### Core Authors
 - **Wei Deng** - Core author; Initiated the IndexTTS project, led the development of the IndexTTS1 data pipeline, model architecture design and training, as well as iterative optimization of the IndexTTS series of models, focusing on fundamental capability building and performance optimization.
 - **Siyi Zhou** – Core author; in IndexTTS2, led model architecture design and training pipeline optimization, focusing on key features such as multilingual and emotional synthesis.
 - **Jingchen Shu** - Core author; worked on overall architecture design, cross-lingual modeling solutions, and training strategy optimization, driving model iteration.
 - **Xun Zhou** - Core author; worked on cross-lingual data processing and experiments, explored multilingual training strategies, and contributed to audio quality improvement and stability evaluation.
 - **Jinchao Wang** - Core author; worked on model development and deployment, building the inference framework and supporting system integration.
 - **Yiquan Zhou** - Core author; contributed to model experiments and validation, and proposed and implemented text-based emotion control.
 - **Yi He** - Core author; contributed to model experiments and validation.
 - **Lu Wang** – Core author; worked on data processing and model evaluation, supporting model training and performance verification.

### Technical Contributors
 - **Yining Wang** - Supporting contributor; contributed to open-source code implementation and maintenance, supporting feature adaptation and community release.
 - **Yong Wu** - Supporting contributor; worked on data processing and experimental support, ensuring data quality and efficiency for model training and iteration.
 - **Yaqin Huang** – Supporting contributor; contributed to systematic model evaluation and effect tracking, providing feedback to support iterative improvements.
 - **Yunhan Xu** – Supporting contributor; provided guidance in recording and data collection, while also offering feedback from a product and operations perspective to improve usability and practical application.
 - **Yuelang Sun** – Supporting contributor; provided professional support in audio recording and data collection, ensuring high-quality data for model training and evaluation.
 - **Yihuang Liang** - Supporting contributor; worked on systematic model evaluation and project promotion, helping IndexTTS expand its reach and engagement.

### Technical Guidance
 - **Huyang Sun** - Provided strong support for the IndexTTS project, ensuring strategic alignment and resource backing.
 - **Bin Xia** - Contributed to the review, optimization, and follow-up of technical solutions, focusing on ensuring model effectiveness.


## 📚 Citation

🌟 If you find our work helpful, please leave us a star and cite our paper.


IndexTTS2:

```
@article{zhou2025indextts2,
  title={IndexTTS2: A Breakthrough in Emotionally Expressive and Duration-Controlled Auto-Regressive Zero-Shot Text-to-Speech},
  author={Siyi Zhou, Yiquan Zhou, Yi He, Xun Zhou, Jinchao Wang, Wei Deng, Jingchen Shu},
  journal={arXiv preprint arXiv:2506.21619},
  year={2025}
}
```


IndexTTS:

```
@article{deng2025indextts,
  title={IndexTTS: An Industrial-Level Controllable and Efficient Zero-Shot Text-To-Speech System},
  author={Wei Deng, Siyi Zhou, Jingchen Shu, Jinchao Wang, Lu Wang},
  journal={arXiv preprint arXiv:2502.05512},
  year={2025},
  doi={10.48550/arXiv.2502.05512},
  url={https://arxiv.org/abs/2502.05512}
}
```
