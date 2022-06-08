Soundcard Latency
=================

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

