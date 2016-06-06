# RoboGif

一款非常方便的 Android 录屏工具。

## 基本条件

* 有 Python2.7 或者 Python 3.X 运行环境
* 环境变量中包含 `adb`
* 环境变量中包含 `ffmpeg` (请尽量使用最新版)

## 配置环境

### 安装 `ffmpeg` 

**OS X**

```
  brew install ffmpeg
```

**Linux**

在 Ubuntu 15.04 或者更高, 你可以使用 `apt`:
```
apt-get install ffmpeg
```
在 Ubuntu 14.04 之前你可以使用 [Ubuntu Multimedia for Trusty PPA](https://launchpad.net/~mc3man/+archive/ubuntu/trusty-media) 来安装新版的ffmpeg.

**Windows**

到 [Zeranoe's static builds](https://ffmpeg.zeranoe.com/builds/) 下载新版的 ffmpeg， 并将 `ffmpeg.exe` 加入环境变量。

## 导入项目

```
pip install robogif
```

## 使用示例:

### 录制gif

```
robogif demo.gif

RoboGif Recorder v1.1.2
Starting recording on <serial>...
Press Ctrl+C to stop recording.
Recording done, downloading file....
5679 KB/s (7036946 bytes in 1.209s)
Converting video to GIF...
Done!
Created demo.gif
```

![GIF example](https://izacus.github.io/RoboGif/images/demo.gif)

### 录制mp4

```
robogif demo.mp4

RoboGif Recorder v1.1.2
Starting recording on 061ffcff0b107aef...
Press Ctrl+C to stop recording.
Recording done, downloading file....
7121 KB/s (1048401 bytes in 0.143s)
Optimizing video...
Done!
Created demo.mp4
```





