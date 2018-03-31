## 安装opencv-python

### 第一种安装opencv完整包(已测试有效)
* 直接安装（解压）[opencv-*.exe](https://sourceforge.net/projects/opencvlibrary/?source=directory),将build目录目录中对应python目录下的`cv.pyd`文件复制python安装目录的`Lib\site-packages\`下；
* 将`opencv\build\bin\opencv_ffmpeg*.dll`添加到环境变量
* 下载[numpy-1.9.2+mkl-cp*.whl](http://www.lfd.uci.edu/~gohlke/pythonlibs/#numpy),在下载目录下执行以下指令即可安装“
```
pip install numpy-1.9.2+mkl-cp*.whl
```

### 第二种，只安装opencv_python模块（待测试）
* 下载对应版本的[numpy](https://www.lfd.uci.edu/~gohlke/pythonlibs/)和[opencv-python](https://www.lfd.uci.edu/~gohlke/pythonlibs/),在下载目录直接安装：
```
pip install numpy-1.12.0+mkl-cp*.whl
pip install opencv_python-*.whl
```

### 测试是否安装成功
```
import cv2

test cv2
print(cv2.__version__)
```