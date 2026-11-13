## 🎯 Projects

### 🎨 Real-Time Rendering

| Project | Description | Stack |
|:--|:--|:--|
| **[LuminaGI](https://github.com/CarlottaSeal/LuminaGI)** | Lumen-style real-time global illumination: surface cache, radiosity, screen-space radiance probes and voxel lighting. SMU Guildhall thesis. | <img src="https://img.shields.io/badge/HLSL-5C2D91?style=flat-square" /> <img src="https://img.shields.io/badge/DX12-006600?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> |
| **[IglooEngine](https://github.com/CarlottaSeal/IglooEngine)** | Custom DX12 rendering engine with a 12-step render pipeline, compute pipeline and job system. The foundation LuminaGI runs on. | <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> <img src="https://img.shields.io/badge/DX12-006600?style=flat-square" /> <img src="https://img.shields.io/badge/HLSL-5C2D91?style=flat-square" /> |
| **[VulkanRTTest](https://github.com/CarlottaSeal/VulkanRTTest)**<br/><img src="https://img.shields.io/badge/WIP-F0A030?style=flat-square" /> | Vulkan KHR ray tracing on Crytek Sponza. ReSTIR DI (Bitterli 2020) with visibility-aware <code>pHat</code> via inline ray queries, plus an SVGF denoiser. | <img src="https://img.shields.io/badge/Vulkan_KHR_RT-AC162C?style=flat-square&logo=vulkan&logoColor=white" /> <img src="https://img.shields.io/badge/GLSL-5586A4?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> |
| **[RedCraft](https://github.com/CarlottaSeal/RedCraft)** | Minecraft-style procedural voxel world generation with terrain algorithms, chunk management and real-time rendering. | <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> |

### ⚡ GPU Compute & ML Kernels

| Project | Description | Stack |
|:--|:--|:--|
| **[FlashAttention-lite](https://github.com/CarlottaSeal/FlashAttention-lite)** | CUDA FlashAttention forward in four profiling-driven versions, v1 to v4 with wmma Tensor Cores, plus a Triton port. Validated on Ada and Blackwell. | <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/Triton-0A0A0A?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> |
| **[LuminaGI-CudaRef](https://github.com/CarlottaSeal/LuminaGI-CudaRef)** | CUDA path tracer (LBVH, NEE, Russian roulette) as ground truth for LuminaGI. PyTorch U-Net denoiser on 8-spp output, <strong>22× faster than 256-spp at 80% of its PSNR gain</strong>. | <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> |

### 🧪 Graphics Testing

| Project | Description | Stack |
|:--|:--|:--|
| **[GfxTestKit](https://github.com/CarlottaSeal/GfxTestKit)** | Config-driven test runner for graphics apps: screenshot diff (PSNR/SSIM), shader compilation tests, memory leak detection, benchmark regression and sanitizer parsing. | <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square" /> <img src="https://img.shields.io/badge/MIT-green?style=flat-square" /> |

### 🤖 Robotics Simulation

| Project | Description | Stack |
|:--|:--|:--|
| **[visual-dr-manipulation](https://github.com/CarlottaSeal/visual-dr-manipulation)**<br/><img src="https://img.shields.io/badge/In_Progress-F0A030?style=flat-square" /> | Which visual randomization actually transfers? Ablation of five DR axes (lighting, material, camera, post-processing, scene geometry) for a vision-based Franka Lift policy, distilled from a state PPO teacher. Each axis maps to a real render-pipeline stage. | <img src="https://img.shields.io/badge/Isaac_Lab-76B900?style=flat-square" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square" /> |

### 🗺️ Planned

- **Vulkan Compute GEMM**: step-by-step GEMM optimization in Vulkan compute shaders, alongside the CUDA work
- **FlashAttention-lite v5**: <code>cp.async</code> + swizzled shared memory in CUDA; Triton backward pass, autotuning, causal masking and PTX analysis
- **CUDA LLM Inference Engine**: every kernel hand-written, running Llama 1B inference end to end

---

## 🛠️ Tech Stack

| | |
|:--|:--|
| **Languages** | <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white" /> <img src="https://img.shields.io/badge/HLSL-5C2D91?style=flat-square" /> <img src="https://img.shields.io/badge/GLSL-5586A4?style=flat-square&logo=opengl&logoColor=white" /> |
| **Graphics APIs** | <img src="https://img.shields.io/badge/DirectX_12-006600?style=flat-square&logo=microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/Vulkan-AC162C?style=flat-square&logo=vulkan&logoColor=white" /> |
| **Tools** | <img src="https://img.shields.io/badge/Visual_Studio-5C2D91?style=flat-square&logo=visual-studio&logoColor=white" /> <img src="https://img.shields.io/badge/Rider-000000?style=flat-square&logo=rider&logoColor=white" /> <img src="https://img.shields.io/badge/PIX-0078D4?style=flat-square&logo=microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/RenderDoc-3C4043?style=flat-square" /> <img src="https://img.shields.io/badge/Perforce-404040?style=flat-square&logo=perforce&logoColor=white" /> <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" /> <img src="https://img.shields.io/badge/ImGui-3C4043?style=flat-square" /> |
| **Testing** | <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" /> <img src="https://img.shields.io/badge/xUnit-239120?style=flat-square&logo=dotnet&logoColor=white" /> <img src="https://img.shields.io/badge/PSNR%2FSSIM_Diff-3C4043?style=flat-square" /> <img src="https://img.shields.io/badge/Sanitizer_Analysis-E34F26?style=flat-square" /> |
| **AI Tools** | <img src="https://img.shields.io/badge/Claude_Code-CC9B7A?style=flat-square&logo=anthropic&logoColor=white" /> <img src="https://img.shields.io/badge/GitHub_Copilot-000000?style=flat-square&logo=githubcopilot&logoColor=white" /> <img src="https://img.shields.io/badge/Cursor-000000?style=flat-square&logo=cursor&logoColor=white" /> <img src="https://img.shields.io/badge/ChatGPT-74AA9C?style=flat-square&logo=openai&logoColor=white" /> |

---

<p align="center">
  <img src="assets/quote.jpg" width="460" alt="无论怎么做，都有很多批评的声音；与其一无所长遭人批评，不如放手创造而招致批评" />
</p>
