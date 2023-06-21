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
2. Micro：INMP-441芯片，
   
  
