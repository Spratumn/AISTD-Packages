## 1. 创建python环境

- 安装conda：推荐使用[Miniconda3](https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda/Miniconda3-latest-Windows-x86.exe)进行python环境的创建管理，下载后双击运行（建议安装到电脑home目录下）；

- 将`C:\Users\用户名\miniconda3\condabin`路径添加到系统环境变量；

- 创建python环境：通过conda创建python环境，这里以runtime为环境名作为示例：

  ```sh
  # 1. 创建名为runtime的python环境并进入dev环境
  conda create -n runtime python=3.9
  conda activate runtime
  # 2. 安装必要库
  conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
  pip install colorlog tqdm lxml opencv-python matplotlib pyyaml onnx imageio thop imageio-ffmpeg pycryptodome PySide6-Fluent-Widgets
  ```

## 2. 打包好的python环境

| 名称                                                         | 依赖                                                     | 备注                |
| ------------------------------------------------------------ | -------------------------------------------------------- | ------------------- |
| [runtime-py39-cuda12.1.zip](https://pan.baidu.com/s/1Yc8m6_Sx4doVZEuKCpN9eQ?pwd=k5br) | [requirements.txt](./requirements/requirements-py39.txt) | 适用软件版本: 3.4.0 |
|                                                              |                                                          |                     |

