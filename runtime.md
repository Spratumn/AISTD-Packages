## 自建Python环境(Windows平台为例)

- 安装conda：推荐使用[Miniconda3](https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda)进行python环境的创建管理，下载后双击运行（建议安装到电脑home目录下）；

- 将`C:\Users\用户名\miniconda3\condabin`路径添加到系统环境变量；

- 创建python环境：通过conda创建python环境，这里以runtime为环境名作为示例：

  ```sh
  # AISTDA
  1. 创建名为aistda的python环境
  conda create -n aistda python=3.12
  conda activate aistda
  # 2. 安装必要库
  pip install torch==2.7.1 torchvision==0.22.1 --index-url https://download.pytorch.org/whl/cu126
  pip install colorlog tqdm lxml opencv-python matplotlib pyyaml onnx imageio thop imageio-ffmpeg pycryptodome docker pyside6
  ```


