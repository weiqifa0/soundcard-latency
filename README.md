Soundcard Latency
=================
## 示意图
这个工具是我同事写的，但是没有示意图，有时候我也经常忘记这个工具怎么使用，我画了一个示意图

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

