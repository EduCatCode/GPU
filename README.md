# GPU

nvidia-smi

+---------------------------------------------------------------------------------------+
| NVIDIA-SMI 536.45                 Driver Version: 536.45       CUDA Version: 12.2     |
|-----------------------------------------+----------------------+----------------------+
| GPU  Name                     TCC/WDDM  | Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp   Perf          Pwr:Usage/Cap |         Memory-Usage | GPU-Util  Compute M. |
|                                         |                      |               MIG M. |
|=========================================+======================+======================|
|   0  NVIDIA GeForce RTX 4060 ...  WDDM  | 00000000:01:00.0  On |                  N/A |
| N/A   50C    P8               2W /  94W |    594MiB /  8188MiB |      2%      Default |
|                                         |                      |                  N/A |
+-----------------------------------------+----------------------+----------------------+


| TensorFlow 版本 | Python 版本 | 編譯器        | 建構工具      | cuDNN | CUDA |
|-----------------|-------------|---------------|---------------|-------|------|
| tensorflow_gpu-2.6.0 | 3.6-3.9 | MSVC 2019 | Bazel 3.7.2 | 8.1   | 11.2 |
| tensorflow_gpu-2.5.0 | 3.6-3.9 | MSVC 2019 | Bazel 3.7.2 | 8.1   | 11.2 |
| tensorflow_gpu-2.4.0 | 3.6-3.8 | MSVC 2019 | Bazel 3.1.0 | 8.0   | 11.0 |
| tensorflow_gpu-2.3.0 | 3.5-3.8 | MSVC 2019 | Bazel 3.1.0 | 7.6   | 10.1 |
| tensorflow_gpu-2.2.0 | 3.5-3.8 | MSVC 2019 | Bazel 2.0.0 | 7.6   | 10.1 |
| tensorflow_gpu-2.1.0 | 3.5-3.7 | MSVC 2019 | Bazel 0.27.1-0.29.1 | 7.6   | 10.1 |
| tensorflow_gpu-2.0.0 | 3.5-3.7 | MSVC 2017 | Bazel 0.26.1 | 7.4   | 10   |
| tensorflow_gpu-1.15.0 | 3.5-3.7 | MSVC 2017 | Bazel 0.26.1 | 7.4   | 10   |
| tensorflow_gpu-1.14.0 | 3.5-3.7 | MSVC 2017 | Bazel 0.24.1-0.25.2 | 7.4   | 10   |
| tensorflow_gpu-1.13.0 | 3.5-3.7 | MSVC 2015 update 3 | Bazel 0.19.0-0.21.0 | 7.4   | 10   |
| tensorflow_gpu-1.12.0 | 3.5-3.6 | MSVC 2015 update 3 | Bazel 0.15.0 | 7.2   | 9.0  |
| tensorflow_gpu-1.11.0 | 3.5-3.6 | MSVC 2015 update 3 | Bazel 0.15.0 | 7     | 9    |
| tensorflow_gpu-1.10.0 | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 7     | 9    |
| tensorflow_gpu-1.9.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 7     | 9    |
| tensorflow_gpu-1.8.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 7     | 9    |
| tensorflow_gpu-1.7.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 7     | 9    |
| tensorflow_gpu-1.6.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 7     | 9    |
| tensorflow_gpu-1.5.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 7     | 9    |
| tensorflow_gpu-1.4.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 6     | 8    |
| tensorflow_gpu-1.3.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 6     | 8    |
| tensorflow_gpu-1.2.0  | 3.5-3.6 | MSVC 2015 update 3 | Cmake v3.6.3 | 5.1   | 8    |
| tensorflow_gpu-1.1.0  | 3.5     | MSVC 2015 update 3 | Cmake v3.6.3 | 5.1   | 8    |
| tensorflow_gpu-1.0.0  | 3.5     | MSVC 2015 update 3 | Cmake v3.6.3 | 5.1   | 8    |


CUDA Toolkit

https://developer.nvidia.com/cuda-toolkit-archive



下載適用於 Windows 的 cuDNN

https://developer.nvidia.com/cudnn


將解壓縮包中的以下檔複製到 NVIDIA cuDNN 目錄中。
複製到 。bin\cudnn*.dllC:\Program Files\NVIDIA\CUDNN\v8.x\bin
複製到 。include\cudnn*.hC:\Program Files\NVIDIA\CUDNN\v8.x\include
複製到 。lib\cudnn*.libC:\Program Files\NVIDIA\CUDNN\v8.x\lib
將以下環境變數設置為指向 cuDNN 所在的位置。若要訪問環境變數的值，請執行以下步驟：$(PATH)
從「開始」功能表打開命令提示符。
鍵入並按 Enter。Run
發出命令。control sysdm.cpl
選擇視窗頂部的「高級」選項卡。
按兩下視窗底部的環境變數。


![image](https://hackmd.io/_uploads/BkE2sIawT.png)
