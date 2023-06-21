# RGB-VHDL-FFT 
![3e7cff98a0a57c3cf85c7b56dcebfcc](https://github.com/ChengchengAncc/RGB-VHDL-FFT/assets/136725382/573addaa-abfe-43a1-8348-ed01e16649c5)
## (English)
# Background
This project is a music spectrum analyzer developed using VHDL language. It utilizes the Altera Cyclone IV E series EP4CE10F17C8 chip.
Here is the show url:<https://www.bilibili.com/video/BV1qA41167bJ/>
Please Q! W! E!
## Main features:
1. Convert the amplitude spectrum of ambient sound to a frequency spectrum using FPGA.
2. Support a 32x16 pixel RGB dot matrix display.
3. Support various types of music visualizations, such as color visualization, bar visualization, and frequency axis quantization (affects the visualization effect).
4. Support mode switching via buttons.
5. Support frequency range: 200Hz to 4.5KHz.
6. Frequency axis quantization methods: Uniform quantization, logarithmic quantization (log2).
## Hardware solution:
1. FPGA: Altera Cyclone IV E series EP4CE10F17C8, an entry-level development board costing around 500 CNY.
2. Microphone: INMP-441 chip, which reads the digital quantized values of ambient sound using the I2S protocol.
3. RGB LEDs: WS2812-B (5050), a 24-bit full-color RGB chip with serial data input. Data timing is crucial, especially the low-level termination for pulling 0.
## Software tools:
Quartus II 18.0.
Utilize Quartus' co-simulation feature to perform functional and timing simulations without the need to install ModelSim separately.
# Installation & Usage:
Download the FPGA project folder and open it in Quartus II by selecting the .qpf file. Ensure that the file path does not contain any Chinese characters, as it may cause the software to freeze during project compilation.
The RGB LED board is provided as an EDA file by Jialichuang. If you do not intend to build it yourself, you can choose a 32x16 RGB LED matrix that meets the requirements. The LED beads should be connected in series per column.
# Maintainers:
Chengcheng.An

## (Chinese)
# 项目背景
项目为基于VHDL语言开发出的音乐频谱仪，使用Altera Cyclone IV E系列的EP4CE10F17C8芯片。展示视频连接如下：<https://www.bilibili.com/video/BV1qA41167bJ/>
请点赞 投币 转发！谢谢
## 主要功能分为：
1. 利用FPGA将环境音的幅度谱转为频谱
2. 支持32*16像素的点阵RGB显示
3. 支持多种层面音乐律动选择，如颜色律动、灯柱律动以及频率轴量化方式（影响律动效果）。
4. 支持按键切换模式
5. 支持频率范围：200Hz~4.5KHz
6. 频率轴量化方式：均匀量化、对数量化（log2）
## 硬件方案：
1. FPGA：Altera Cyclone IV E系列的EP4CE10F17C8，价格500元左右的入门开发板
2. Micro：INMP-441芯片，采用I2S协议读取环境音的数字量化值
3. RGB：WS2812-B（5050），24bit全彩RGB芯片，串行数据输入，数据时序非常重要，尤其注意低电平拉0的结束符
## 软件工具：
1. Quartus II 18.0
2. 利用Quartus的联合仿真，无需安装Modelsim即可在Quartus II内进行功能、时序仿真

# 安装 & 使用
1. FPGA工程文件夹下载后直接在Quartus II中open project，选择qpf文件即可，注意路径中不要包含任何中文，否则软件进行工程编译时会卡死
2. RGB灯板为嘉立创EDA文件，若无意自制，可自选32*16-RGB灯阵即可，要求16为行数，32为列数，以列为单位进行灯珠串联

# 贡献者
Chengcheng.An
   
  
