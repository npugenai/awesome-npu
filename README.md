<div align="center">

<svg width="800" height="120" viewBox="0 0 800 120" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#1a1625"/>
      <stop offset="100%" style="stop-color:#2d2a47"/>
    </linearGradient>
    <linearGradient id="tg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#a18cd1"/>
      <stop offset="100%" style="stop-color:#d1c4e9"/>
    </linearGradient>
  </defs>
  <rect width="800" height="120" rx="16" fill="url(#bg)"/>
  <rect width="800" height="120" rx="16" fill="none" stroke="#a18cd1" stroke-width="1" stroke-opacity="0.3"/>
  <text x="400" y="52" font-family="Segoe UI, Arial, sans-serif" font-size="30" font-weight="800" fill="url(#tg)" text-anchor="middle">Awesome NPU</text>
  <text x="400" y="85" font-family="Segoe UI, Arial, sans-serif" font-size="14" fill="#b0bec5" text-anchor="middle">A curated list of NPU development resources for on-device AI</text>
</svg>

<br/>

[![npugenai.com](https://img.shields.io/badge/🌐_npugenai.com-a18cd1?style=for-the-badge&logoColor=white)](https://www.npugenai.com)
[![npubenchmark.org](https://img.shields.io/badge/📊_NPU_Benchmark-8a73b8?style=for-the-badge&logoColor=white)](https://www.npubenchmark.org)
[![Awesome](https://img.shields.io/badge/Awesome-List-d1c4e9?style=for-the-badge)](https://github.com/sindresorhus/awesome)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-6dcf8e?style=for-the-badge)](https://github.com/npugenai/awesome-npu/pulls)

</div>

---

## Contents

- [SDKs & Frameworks](#sdks--frameworks)
- [Models](#models)
- [Tools](#tools)
- [Guides & Tutorials](#guides--tutorials)
- [Papers](#papers)
- [Community](#community)

---

## SDKs & Frameworks

| Name | Vendor | Platform | Description |
|---|---|---|---|
| [ONNX Runtime](https://onnxruntime.ai) | Microsoft | AMD · Intel · Qualcomm | Cross-platform inference engine with NPU execution providers |
| [Intel OpenVINO](https://docs.openvino.ai) | Intel | Intel NPU | Open-source inference toolkit optimized for Intel NPU |
| [AMD Ryzen AI SDK](https://ryzenai.docs.amd.com) | AMD | AMD XDNA | Developer SDK for Ryzen AI series NPUs with ONNX Runtime integration |
| [Qualcomm QNN SDK](https://qpm.qualcomm.com) | Qualcomm | Qualcomm Hexagon | Neural Network SDK for Snapdragon NPU deployment |
| [DirectML](https://learn.microsoft.com/en-us/windows/ai/directml) | Microsoft | AMD · Intel · Qualcomm | Low-level ML API for Windows NPU acceleration |
| [Windows AI APIs](https://learn.microsoft.com/en-us/windows/ai/) | Microsoft | Copilot+ PC | Built-in Windows APIs including Phi Silica and WinML |
| [Microsoft Olive](https://github.com/microsoft/Olive) | Microsoft | All | Hardware-aware model optimization and quantization toolchain |

---

## Models

| Model | Format | Precision | Platform | Source |
|---|---|---|---|---|
| LLaMA 3.2 1B / 3B | ONNX / GGUF | INT4 | AMD · Intel | [HuggingFace](https://huggingface.co/meta-llama) |
| Phi-3.5 Mini | ONNX | INT4 | All | [HuggingFace](https://huggingface.co/microsoft/Phi-3.5-mini-instruct) |
| Phi-3 Mini 4K | ONNX | INT4 | All | [HuggingFace](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct-onnx) |
| Whisper Large v3 | ONNX | INT8 | AMD · Intel · Qualcomm | [HuggingFace](https://huggingface.co/openai/whisper-large-v3) |
| Stable Diffusion XL Turbo | ONNX | FP16 | AMD · Intel · Qualcomm | [HuggingFace](https://huggingface.co/stabilityai) |
| Mistral 7B | GGUF | INT4 | AMD · Intel | [HuggingFace](https://huggingface.co/mistralai) |

---

## Tools

| Name | Description | Link |
|---|---|---|
| **NPU Benchmark** | Universal cross-platform NPU benchmark tool | [npubenchmark.org](https://www.npubenchmark.org) |
| **Netron** | ONNX / TensorFlow / CoreML model visualizer | [netron.app](https://netron.app) |
| **AMD uProf** | CPU/NPU performance profiler for AMD platforms | [AMD](https://www.amd.com/en/developer/uprof.html) |
| **Intel VTune** | Performance profiler with Intel NPU support | [Intel](https://www.intel.com/content/www/us/en/developer/tools/oneapi/vtune-profiler.html) |
| **ONNX Model Zoo** | Pre-trained ONNX models ready for NPU deployment | [GitHub](https://github.com/onnx/models) |

---

## Guides & Tutorials

| Title | Platform | Level |
|---|---|---|
| [Getting Started with AMD Ryzen AI SDK](https://ryzenai.docs.amd.com/en/latest/inst.html) | AMD XDNA | Beginner |
| [Deploy LLM with ONNX Runtime on NPU](https://onnxruntime.ai/docs/execution-providers/DirectML-ExecutionProvider.html) | All | Intermediate |
| [Quantize Models with Olive](https://github.com/microsoft/Olive/tree/main/examples) | All | Intermediate |
| [Intel NPU with OpenVINO](https://docs.openvino.ai/2024/openvino-workflow/running-inference/inference-devices-and-modes/npu-device.html) | Intel NPU | Intermediate |
| [Qualcomm AI Hub Model Deployment](https://aihub.qualcomm.com/docs) | Qualcomm | Intermediate |
| [Windows Copilot+ PC AI Dev Guide](https://learn.microsoft.com/en-us/windows/ai/npu-developers/) | All | Beginner |

---

## Papers

| Title | Year | Topic |
|---|---|---|
| [AWQ: Activation-aware Weight Quantization for LLM](https://arxiv.org/abs/2306.00978) | 2023 | INT4 Quantization |
| [GPTQ: Accurate Post-Training Quantization for GPT](https://arxiv.org/abs/2210.17323) | 2022 | LLM Quantization |
| [SmoothQuant: Accurate and Efficient Post-Training Quantization](https://arxiv.org/abs/2211.10438) | 2022 | INT8 Quantization |
| [MLC-LLM: Universal LLM Deployment](https://arxiv.org/abs/2306.05176) | 2023 | Edge Deployment |

---

## Community

- 🌐 **Community Hub** → [npugenai.com](https://www.npugenai.com)
- 📊 **Benchmark Tool** → [npubenchmark.org](https://www.npubenchmark.org)
- 💬 **Discord** → *Coming Soon*
- 📬 **Newsletter** → *Coming Soon*
- 🐙 **GitHub** → [github.com/npugenai](https://github.com/npugenai)

---

## Contributing

PRs are welcome! Please read the contribution guidelines before submitting.

1. Fork this repository
2. Add your resource in the appropriate section
3. Make sure the link is working and the description is accurate
4. Submit a pull request

---

<div align="center">
<sub>Maintained by <a href="https://www.npugenai.com">NPU GenAI Community</a> · Built with 💜</sub>
</div>
