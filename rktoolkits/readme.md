## Docker软件安装

### Windows平台

1. 启用相关功能：依次进入 控制面板-程序-程序和功能-启用或关闭Windows功能，选中"Hyper-V"和"适用于 Linux 的 Windows 子系统"，等待完成并重启电脑
2. 电脑重启后，打开"终端管理员"并执行命令："wsl --update"
3. 下载并安装Docker-Desktop，安装完成后启动Docker-Desktop

### Linux平台

1. 安装docker-ce

```bash
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update

# Install docker-ce
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

```
2. 设置docker命令权,避免使用sudo命令执行docker

```bash
sudo usermod -aG docker ${USER}
sudo gpasswd -a ${USER} docker
newgrp docker
```


## RKNN模型转换工具-Docker镜像包

| 镜像名称             | 下载地址                                                     | 备注                |
| -------------------- | ------------------------------------------------------------ | ------------------- |
| rktoolkit-1.7.3.zip  | [百度云盘](https://pan.baidu.com/s/1aMsSJ80oWWBwez5Z5u30TA?pwd=yyp9) / [Google Drive](https://drive.google.com/file/d/1qUUQnhVa2jLmUtj50O5qp5bwz4uKZV2K) | 适用软件版本: 3.4.0 |
| rktoolkit2-2.3.0.zip | [百度云盘](https://pan.baidu.com/s/1ejvRK2-_FM6jvgOUsEMowg?pwd=n3a3) / [Google Drive](https://drive.google.com/file/d/1df7_cQ0p99AeFlKzQCsmDInaglvFbU3q) | 适用软件版本: 3.4.0 |
|                      |                                                              |                     |



## 模型重置升级包

| 升级包名称        | 下载地址                                                     | 备注                |
| ----------------- | ------------------------------------------------------------ | ------------------- |
| model_reseter.swu | [百度云盘](https://pan.baidu.com/s/1VdJT4ecLG6cAQI40Sk5l7w?pwd=b6ay) / [Google Drive](https://drive.google.com/file/d/1a48_ZUVyrHy_B3tgt2C64CYVcnwkNjLa) | 适用软件版本: 3.4.0 |
|                   |                                                              |                     |


