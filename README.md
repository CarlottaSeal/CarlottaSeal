## 🎯 Projects

### 🎨 Real-Time Rendering

<table>
  <tr><th width="160" align="left">Project</th><th width="420" align="left">Description</th><th width="180" align="left">Stack</th></tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/LuminaGI">LuminaGI</a></b></td>
    <td width="420">Lumen-style real-time global illumination: surface cache, radiosity, screen-space radiance probes and voxel lighting. SMU Guildhall thesis.</td>
    <td width="180"><img src="https://img.shields.io/badge/HLSL-5C2D91?style=flat-square" /> <img src="https://img.shields.io/badge/DX12-006600?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/IglooEngine">IglooEngine</a></b></td>
    <td width="420">Custom DX12 rendering engine with a 12-step render pipeline, compute pipeline and job system. The foundation LuminaGI runs on.</td>
    <td width="180"><img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /> <img src="https://img.shields.io/badge/DX12-006600?style=flat-square" /> <img src="https://img.shields.io/badge/HLSL-5C2D91?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/VulkanRTTest">VulkanRTTest</a></b></td>
    <td width="420">Vulkan KHR ray tracing on Crytek Sponza. ReSTIR DI (Bitterli 2020) with visibility-aware <code>pHat</code> via inline ray queries, plus an SVGF denoiser.</td>
    <td width="180"><img src="https://img.shields.io/badge/Vulkan_KHR_RT-AC162C?style=flat-square&logo=vulkan&logoColor=white" /> <img src="https://img.shields.io/badge/GLSL-5586A4?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/RedCraft">RedCraft</a></b></td>
    <td width="420">Minecraft-style procedural voxel world generation with terrain algorithms, chunk management and real-time rendering.</td>
    <td width="180"><img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
</table>

### 🤖 Robotics Simulation

<table>
  <tr><th width="160" align="left">Project</th><th width="420" align="left">Description</th><th width="180" align="left">Stack</th></tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/visual-dr-manipulation">visual-dr-manipulation</a></b><br/><img src="https://img.shields.io/badge/In_Progress-F0A030?style=flat-square" /></td>
    <td width="420">Which visual randomization actually transfers? Ablation of five DR axes (lighting, material, camera, post-processing, scene geometry) for a vision-based Franka Lift policy, distilled from a state PPO teacher. Each axis maps to a real render-pipeline stage.</td>
    <td width="180"><img src="https://img.shields.io/badge/Isaac_Lab-76B900?style=flat-square" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square" /></td>
  </tr>
</table>

### ⚡ GPU Compute & AI Kernels

<table>
  <tr><th width="160" align="left">Project</th><th width="420" align="left">Description</th><th width="180" align="left">Stack</th></tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/FlashAttention-lite">FlashAttention-lite</a></b></td>
    <td width="420">CUDA FlashAttention from scratch in six profiling-driven versions (naive → wmma → <code>mma.sync</code> + register-resident S/P/O + XOR swizzle shmem), plus a Triton port with multi-head, causal and backward pass. Validated on Ada and Blackwell.</td>
    <td width="180"><img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/Triton-0A0A0A?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/llama-cuda-inference">llama-cuda-inference</a></b></td>
    <td width="420">CUDA inference engine for Llama 3.2 1B — every kernel hand-written, no cuBLAS/cuDNN. GEMM (naive → tiled → wmma Tensor Cores), FlashAttention, RMSNorm, RoPE, SiLU×Mul. Greedy output matches HF transformers token-for-token.</td>
    <td width="180"><img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/vulkan-gemm">vulkan-gemm</a></b></td>
    <td width="420">FP32 SGEMM as Vulkan compute shaders, one optimization per kernel (naive → smem tiling → vec4 register blocking → subgroup shuffle), benchmarked against cuBLAS.</td>
    <td width="180"><img src="https://img.shields.io/badge/Vulkan_Compute-AC162C?style=flat-square&logo=vulkan&logoColor=white" /> <img src="https://img.shields.io/badge/GLSL-5586A4?style=flat-square" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/neural-rendering-cuda">neural-rendering-cuda</a></b></td>
    <td width="420">GPU kernel work on neural rendering: 3DGS rasterizer optimization (<b>1.7× training speedup</b>, PSNR within 0.03 dB), Instant-NGP from scratch (hash encoding <b>12.6× faster</b> than PyTorch reference), and a differentiable soft rasterizer.</td>
    <td width="180"><img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/LuminaGI-CudaRef">LuminaGI-CudaRef</a></b></td>
    <td width="420">CUDA path tracer (LBVH, NEE, Russian roulette) as ground truth for LuminaGI. PyTorch U-Net denoiser on 8-spp output, <b>22× faster than 256-spp at 80% of its PSNR gain</b>.</td>
    <td width="180"><img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/C++-00599C?style=flat-square" /></td>
  </tr>
</table>

### 🧪 Graphics Testing

<table>
  <tr><th width="160" align="left">Project</th><th width="420" align="left">Description</th><th width="180" align="left">Stack</th></tr>
  <tr>
    <td width="160"><b><a href="https://github.com/CarlottaSeal/GfxTestKit">GfxTestKit</a></b></td>
    <td width="420">Config-driven test runner for graphics apps: screenshot diff (PSNR/SSIM), shader compilation tests, memory leak detection, benchmark regression and sanitizer parsing.</td>
    <td width="180"><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square" /> <img src="https://img.shields.io/badge/MIT-green?style=flat-square" /></td>
  </tr>
</table>

### 🗺️ Next

- **Triton compiler contributions**: bug fixes, benchmarks and backend optimizations in C++/MLIR

---

## 🛠️ Tech Stack

| | |
|:--|:--|
| **Languages** | <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white" /> <img src="https://img.shields.io/badge/HLSL-5C2D91?style=flat-square" /> <img src="https://img.shields.io/badge/GLSL-5586A4?style=flat-square&logo=opengl&logoColor=white" /> |
| **GPU** | <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/Triton-0A0A0A?style=flat-square" /> <img src="https://img.shields.io/badge/DirectX_12-006600?style=flat-square&logo=microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/Vulkan-AC162C?style=flat-square&logo=vulkan&logoColor=white" /> |
| **Profiling** | <img src="https://img.shields.io/badge/NSight_Compute-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/NSight_Systems-76B900?style=flat-square&logo=nvidia&logoColor=white" /> <img src="https://img.shields.io/badge/PIX-0078D4?style=flat-square&logo=microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/RenderDoc-3C4043?style=flat-square" /> |
| **Tools** | <img src="https://img.shields.io/badge/Visual_Studio-5C2D91?style=flat-square&logo=visual-studio&logoColor=white" /> <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" /> <img src="https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white" /> <img src="https://img.shields.io/badge/ImGui-3C4043?style=flat-square" /> |
| **Testing** | <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" /> <img src="https://img.shields.io/badge/compute--sanitizer-76B900?style=flat-square" /> <img src="https://img.shields.io/badge/PSNR%2FSSIM_Diff-3C4043?style=flat-square" /> |

---

<p align="center">
  <img src="assets/quote.jpg" width="460" alt="无论怎么做，都有很多批评的声音；与其一无所长遭人批评，不如放手创造而招致批评" />
</p>
