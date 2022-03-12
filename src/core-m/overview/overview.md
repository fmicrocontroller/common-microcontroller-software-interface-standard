# 概述

------

`CMSIS-Core(Cortex-M)`实现了`Cortex-M`设备的基本运行时，并允许用户处理器内核和设备外设。它详细定义了：

- `Hardware Abstraction Layer(HAL)`：对`Cortex-M`处理器寄存器标准化地定义出了`SysTick`、`NVIC`、系统控制寄存器、`MPU`寄存器、`FPU`寄存器、内核访问函数。
- `System exception names`：不存在兼容性问题的系统异常接口。
- `Methods to organize header files`：便于学习新的`Cortex-M`微控制器产品并提高软件的可移植性。这包括特定设备中断的命名约定。
- `Methods for system initialization`：给`MCU`厂商使用的。例如，标准化的`SystemInit()`函数对于配置设备的时钟系统是必不可少的。
- `Intrinsic function`：用来生成标准`C`语言不支持的`CPU`指令集。
- 用于确定系统始终频率的变量，可简化`SysTick`定时器的设置。

以下章节提供有关`CMSIS-Core(Cortex-M)`的详细信息：

- [在嵌入式应用中使用`CMSIS`]：描述创建项目并展示一个简单的例子。
- [在`Armv8-M`中使用`TrustZone`]：描述如何使用`Armv8-M`结构中的安全插件。
- [`CMSIS-Core`设备样板代码]：详细描述了`CMSIS-Core(Cortex-M)`中的文件并解释如何为硬件厂商适配这些样板代码。
- [MISRA-C Deviations]：描述违反`MISRA`标注的情况。
- [Reference]：详细地描述了`Device Header File <device.h>`的特性和函数。
- [Data Structures]：详细地描述了`Device Header File <device.h>`的数据结构。
