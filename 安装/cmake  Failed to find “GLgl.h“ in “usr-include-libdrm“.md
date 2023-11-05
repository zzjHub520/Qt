在 安装 cmake 中，执行 ./bootstrap 时出现  Failed to find "GL/gl.h" in "/usr/include/libdrm"

解决办法：

```sh
sudo yum install mesa-libGL-devel mesa-libGLU-devel -y
sudo apt install mesa-common-dev libglu1-mesa-dev -y
```

然后删除 CMakeCache.txt，继续执行 ./bootstrap。