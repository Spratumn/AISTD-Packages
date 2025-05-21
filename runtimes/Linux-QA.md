## 运行错误

### 1. 运行main.elf，出现如下qt.qpa.plugin相关错误
```
qt.qpa.plugin: From 6.5.0, xcb-cursor0 or libxcb-cursor0 is needed to load the Qt xcb platform plugin.
qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "/home/xxx/miniconda3/envs/runtime/lib/python3.9/site-packages/cv2/qt/plugins" even though it was found.
This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.

Available platform plugins are: xcb, eglfs, vkkhrdisplay, wayland, vnc, minimalegl, linuxfb, minimal, wayland-egl, offscreen.

Aborted (core dumped)
```

**解决方法：**

```bash
sudo apt-get install libxcb-cursor0
```

### 2. 在应用部署中，在已安装好docker的情况下点击加载镜像仍提示docker软件未打开

**解决方法：**
参考[rktoolkit-readme](rktoolkits\readme.md)，设置docker命令权,避免使用sudo命令执行docker

### 3. Linux端用户工具安装和授权[参考](https://h.virbox.com/docs/usermanual/tools/Virbox-UserTool/VirboxLM-User-License-Tool-Linux)
