# Cortex-M4-coding
# 这里只给出了中断处理函数和LED控制代码。
main.c是中断处理函数和LED控制代码。
commenting是对CMSIS的启动函数startup.s的注释
我们需要在STM32CubeIDE中创建一个新的工程。选择你的板子型号，打开CubeMX配置工具，进行如下配置：
在GPIO设置中，将PA0配置为输入模式，PD12配置为输出模式。
在NVIC设置中，使能EXTI0中断，并将其优先级设置为较高的值，例如0或1。
在时钟设置中，使能GPIOA和GPIOD时钟。
完成配置后，生成代码并打开main.c文件。我们将在其中添加中断处理函数和LED控制代码。
