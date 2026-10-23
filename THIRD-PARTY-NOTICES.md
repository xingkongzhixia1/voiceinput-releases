# 第三方组件与数据来源声明

本软件（输控工作台 / VoiceInput）为闭源专有软件，但包含或依赖以下第三方组件与数据。各组件按其原作者许可证使用，本软件自身的专有许可不改变这些组件的许可条件。

## 一、随安装包分发的组件

| 组件 | 版本 | 许可证 | 版权 |
| --- | --- | --- | --- |
| NAudio | 2.2.1 | MIT | © Mark Heath |
| org.k2fsa.sherpa.onnx | 1.13.8 | Apache-2.0 | © k2-fsa / sherpa-onnx contributors |
| BlueBird.Pinyins | 1.3.0 | MIT | © BlueBird.Pinyins 作者 |
| System.Speech | 8.0.0 | MIT | © .NET Foundation and Contributors |
| .NET 8 运行时（自包含发布） | 8.x | MIT | © .NET Foundation and Contributors |
| ONNX Runtime（随 sherpa-onnx） | — | MIT | © Microsoft Corporation |
| Inno Setup（安装包外壳） | 6 | Inno Setup License | © Jordan Russell |

- MIT 许可允许使用、复制、修改、合并、发布、分发、再许可及销售副本，但须在副本中保留版权声明与本许可声明；软件按「现状」提供，不提供担保。完整文本：<https://opensource.org/license/mit>
- Apache-2.0 许可允许使用、修改、分发，但须保留版权与许可声明、标明修改并附许可证副本。完整文本：<https://www.apache.org/licenses/LICENSE-2.0>

## 二、随程序内嵌的数据

### 同音词库 `homophone-words.tsv.gz`

由以下来源生成，整体以 **CC BY-SA 4.0** 提供：

- CC-CEDICT 词条与拼音：© MDBG / CC-CEDICT contributors，**CC BY-SA 4.0**
- jieba 词典词频：© 2013 Sun Junyi，**MIT**
- pinyin-pro 生成的读音：**MIT**（仅构建时使用，不随安装包分发）

建议署名文字：

> 同音词数据来自 CC-CEDICT（© MDBG / CC-CEDICT contributors，CC BY-SA 4.0）、
> jieba 词典（© 2013 Sun Junyi，MIT）与 pinyin-pro（MIT，仅构建时使用）。

说明：该数据集适用独立的 CC BY-SA 4.0 许可，不改变本软件整体的专有许可；复用该数据须遵守 CC BY-SA 4.0。

### 在线补充词库

用户主动触发更新时，从 jieba `dict.txt`（MIT）下载，仅保存在本机 `%LOCALAPPDATA%\VoiceInput\homophone-extra.tsv.gz`。

## 三、不随安装包分发的模型

离线识别模型由用户首次使用时按需下载，版权与许可归各模型作者：

- `csukuangfj/sherpa-onnx-sense-voice-zh-en-ja-ko-yue-2024-07-17`
- `csukuangfj/sherpa-onnx-streaming-paraformer-bilingual-zh-en`
- `csukuangfj2/sherpa-onnx-qwen3-asr-0.6B-int8-2026-03-25`

使用前请阅读对应仓库的 LICENSE。本软件不重新分发这些模型文件。

## 四、在线服务

在线识别、AI 纠错、翻译由用户自行配置的第三方服务提供，相关条款与隐私政策由该服务方负责。
