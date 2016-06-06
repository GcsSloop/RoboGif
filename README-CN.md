# RoboGif

一款非常方便的 Android 录屏工具,在之前的版本中robogif录制出来的文件非常大，但新版已经修改优化，录制出来的文件大小还不错。

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

## 支持参数

参数   | 示例                                      | 解释
-------|-------------------------------------------|-------------------------------------------------
`-i`   | `robogif -i inputfile.mp4 outputfile.gif` | 将输入的mp4文件转换为gif
`-s`   | `robogif -s 300 output.gif`               | 指定输出文件的大小(图片或视频的宽度，默认是480)
`-f`   | `robogif -f 20 output.gif`                | 指定输出文件的帧率(gif默认是15，mp4默认是40)

<br/>
<br/>
<br/>



