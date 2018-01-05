# rtlmm

_Created by Pete Schwamb. Code is released under MIT license._

**rtlmm** is software to sniff minimed RF packets using a RTLSDR dongle

This work is inspired by and partially based on Evariste Courjaud's great tool: https://github.com/F5OEO/rtlomni

# Prerequisites

* liquid-dsp: On mac, you can `brew install liquid-dsp`.  On linux systems, you must build from source: https://github.com/jgaeddert/liquid-dsp/

# Installation
```sh

git clone https://github.com/ps2/rtlmm
cd rtlmm
make

#Install rtl-sdr driver and utilities (rtl_test, rtl_sdr ...)
sudo apt-get install rtl-sdr

```

# Launching rtlmm
you can launch :
```sh
./rtlmm some_file.cu8
```
It outputs messages from a RF sample file included in the folder.

For live message recording, there is a script
```sh
./recordiq.sh
```
