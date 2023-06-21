# RGB-VHDL-FFT
# Background
项目为基于VHDL语言开发出的音乐频谱仪，使用Altera Cyclone IV E系列的EP4CE10F17C8芯片。
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

# Install & Usage
1. FPGA工程文件夹下载后直接在Quartus II中open project，选择qpf文件即可，注意路径中不要包含任何中文，否则软件进行工程编译时会卡死
2. RGB灯板为嘉立创EDA文件，若无意自制，可自选32*16-RGB灯阵即可，要求16为行数，32为列数，以列为单位进行灯珠串联

# Maintainers
Chengcheng.An
   
  
