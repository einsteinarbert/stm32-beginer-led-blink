# Starter - LED blinking with STM32
> Giới thiệu lập trình và ví dụ led STM32: https://www.youtube.com/watch?v=dILi7hPyDAU

> STM32F412RE: https://github.com/WeActStudio/WeActStudio.STM32F4_64Pin_CoreBoard

> ./Hardware/WeAct-STM32F4_64PIN-CoreBoard_V10 Board Shape 外形.pdf

> ./Doc/RM0402 STM32F412 Reference manual.pdf

> Model STM32: stm32f412ret6 (made by WeAct Studio)

## Build & Run
1. Generage code in STM32CubeMX app
2. Edit code & Build hex file in MDK-ARM uVision to hex file, for ex: `led-blink.hex`
3. Copy hex file to `X:\workspace\0.FPV\stm32f412ret6\WeActStudio.STM32F4_64Pin_CoreBoard\Tools\WeAct Studio Download Tool_V1.2`
4. Press & hold B0 switch key in board and connect to Computer => red led showing up
5. Run `WeAct Studio USB Download Tool.bat` and input `led-blink.hex` to console => enter to `download` hex file to STM32 MCU

## Circuit
> This circuit below are: sink source circuit style

** Mạch bên dưới vẽ theo kiểu mạch sink dòng, nó cho phép nguồn đi qua tải trước khi trở về chân IC => làm cho IC không bị cháy, hơn nữa đủ nguồn nuôi tải, IC chỉ có vai trò đóng mở chân (-) của mạch để điều khiển I/O

![Led-blink with STM32](circuit-1.png)
