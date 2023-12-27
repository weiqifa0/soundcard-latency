Soundcard Latency
=================
## 示意图
这个工具是我同事写的，但是没有示意图，有时候我也经常忘记这个工具怎么使用，我画了一个示意图

+ 首先speaker 也是有麦克风的，我们测试的时候，先需要把speaker的延迟测试出来，就是音频发送出去，再采集回来的时间差。
+ 再次，我们把播放设置成speaker 采集设置成Microphone ，这样把新测试到的延时数据，减去上面speaker自身的延时，就是Microphone的上行延时加上空气传播的时间延时。
+ 空气传播你把两个设备放得比较近，可以忽略


![image](https://github.com/weiqifa0/soundcard-latency/assets/11375905/332b73ff-4e7e-4e78-b6ec-6c5712d426bd)




[![build](https://github.com/xiongyihui/soundcard-latency/actions/workflows/build.yml/badge.svg)](https://github.com/xiongyihui/soundcard-latency/actions/workflows/build.yml)

A tool to check the latency of a sound card.

![](screenshot.png)

Download the application from [![build](https://github.com/xiongyihui/soundcard-latency/actions/workflows/build.yml/badge.svg)](https://github.com/xiongyihui/soundcard-latency/actions/workflows/build.yml).

## Advance
### Requirements
+ python3
+ numpy
+ python-sounddevice
+ samplerate
+ matplotlib
+ pip3 install numpy
+ pip3 install matplotlib
+ pip3 install samplerate
+ pip3 install sounddevice

### Get started with `latency.py`
+   Measure the default input and output devices.

    ```
    python3 latency.py
    ```

+   Measure two specified devices

    1.  list all devices

        ```
        python3 -m sounddevice
        ```

    2.  use the indexes to specify two devices

        ```
        python3 latency 1 2
        ```

