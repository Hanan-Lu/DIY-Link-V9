# DIY Link V9

此项目为一个Clone J-Link V9 的硬件项目，并进行了一些优化升级。

## 功能特点

    支持Jlink Base的全部功能，在此基础上增加一键切换内外参考电压功能，免去拆壳的繁琐

+ 支持电平转换，电压范围1.2~5V

+ 支持5V VOUT输出，输出采用MOS管控制，损耗更小

+ 优化电压跟踪器，真正的支持5V I/O电平，工作更稳定

+ 支持固件升级

+ 支持VCOM，(注意，开启VCOM后只能使用SWD模式)

+ 支持USB A to C及 C to C线

+ 用料扎实，布局合理，器件均为一线大厂(ST、Microchip、Nexperia、SG-Micro、Torex、Cvilux、JST/CJT、YXC、Yageo/Samsung 等)

+ PCB为无铅工艺

+ 接口线序采用ARM推荐的10Pin JTAG接口

+ 壳体采用CC-Debugger调试器外壳，可自行淘宝购买

## 实物图

!["正面图"](https://github.com/Hanan-Lu/DIY-Link-V9/blob/main/04%20-%20%E5%AE%9E%E7%89%A9%E5%9B%BE/PCBA%20-%20TOP.jpg "正面图")
!["背面图"](https://github.com/Hanan-Lu/DIY-Link-V9/blob/main/04%20-%20%E5%AE%9E%E7%89%A9%E5%9B%BE/PCBA%20-%20Bottom.jpg "背面图")
!["装配图"](https://github.com/Hanan-Lu/DIY-Link-V9/blob/main/04%20-%20%E5%AE%9E%E7%89%A9%E5%9B%BE/Assembly.jpg "装配图")

## 注意事项

+ 开启内部参考电压后，VREF引脚上会输出一个3.3V电压，但是此电压不能带大负载，因为其内阻较大(默认为5.1±1% Ohm, 目的为保护作用)，因此如希望使用调试器供电建议使用VOUT引脚(5V输出)

+ 总电流消耗建议小于500mA ( 输入自恢复保险丝规格为0.5A/6V/0805 )
