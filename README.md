# ubuntu-xfce4-vnc

### 安装了xfce4 和 x11vnc 的 docker镜像

基于ubuntu:latest镜像构建
安装了以下组件
- x11vnc
- xfce4 xfce4-terminal
- Xvfb


使用`docker build`构建镜像
```
cd ubuntu-xfce4-vnc
docker build --rm -t ubuntu-xfce4-vnc .
```

启动镜像 VNC默认端口`5901`
```
docker run -it -d -p 5901:5901 ubuntu-xfce4-vnc
```

使用VNC Viewer连接 默认密码`123456` 分辨率`1366x768`

