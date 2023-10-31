# README

```bash

conda create -n sd1 python=3.10.6
conda init powershell
conda activate sd1

pip install torch==2.1.0

# windows
$ENV:LIBTORCH_USE_PYTORCH=1

cargo run --example stable-diffusion --features clap -- --prompt "A rusty robot holding a fire torch."

```

or

```bash

# 查看 CUDA 版本
nvidia-smi

```

显示：` CUDA Version: 12.1`

在 https://pytorch.org/get-started/locally/ 下载对应 libtorch: `wget https://download.pytorch.org/libtorch/cu121/libtorch-win-shared-with-deps-2.1.0%2Bcu121.zip`，自行解压缩。

```bash

$Env:LIBTORCH = "D:\libs\libtorch"
$Env:Path += ";D:\libs\libtorch\lib"

cargo run --example stable-diffusion --features clap -- --prompt "A rusty robot holding a fire torch."

```

## 模型讲解

- clip
- unet
- vae

[手写 Stable Diffusion](https://zhuanlan.zhihu.com/p/621325215)
