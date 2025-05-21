## 1. 创建python环境(Windows平台为例)

- 安装conda：推荐使用[Miniconda3](https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda)进行python环境的创建管理，下载后双击运行（建议安装到电脑home目录下）；

- 将`C:\Users\用户名\miniconda3\condabin`路径添加到系统环境变量；

- 创建python环境：通过conda创建python环境，这里以runtime为环境名作为示例：

  ```sh
  # 1. 创建名为runtime的python环境
  conda create -n runtime python=3.9
  conda activate runtime
  # 2. 安装必要库
  conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
  pip install colorlog tqdm lxml opencv-python matplotlib pyyaml onnx imageio thop imageio-ffmpeg pycryptodome PySide6-Fluent-Widgets
  ```

## 2. 打包好的python环境

| 名称                  | 下载地址                                                     | 依赖                                                     | 备注                |
| --------------------- | ------------------------------------------------------------ | -------------------------------------------------------- | ------------------- |
| runtime-py39-cuda12.1.zip | [百度云盘](https://pan.baidu.com/s/1Yc8m6_Sx4doVZEuKCpN9eQ?pwd=k5br) / [Google Drive](https://drive.google.com/file/d/13Jg-Mf56iJ1Qn4ylW76vf70dbWsE7njO) | [requirements.txt](./requirements/requirements-py39.txt) | Windows平台,适用软件版本: 3.4.0 |
|                       |                                                              |                                                          |                     |
| runtime-py39-cuda12.1.tar.xz | [百度云盘](https://pan.baidu.com/s/1gsi5JznUWXW5Dt2ebTmkIA?pwd=n84y) / [Google Drive](https://drive.google.com/file/d/1H6IiFi_Wi8FOp2otzB0AHppBHFDG95QA) | [requirements.txt](./requirements/requirements-py39.txt) | Linux平台,适用软件版本: 3.4.0 |
|                       |                                                              |                                                          |                     |

