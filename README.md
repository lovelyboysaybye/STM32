
# NUCLEO F072RB
Measuring time of pressing button (seconds) and sending result to terminal through UART.

# Requirements
* NUCLEO F072RB
* UART-USB (for example FTDI232)
* STM32CUBEMX
* keli Vision (MDK-ARM > v5.27)

# Configurations
[STM_PINS](IMG/STM_PINS.jpg)
* USART4
- BaundRate: __115100 bit/sec__
* TIM16
- Prescaler: __48000- 1__ (that's mean, that 48MHz divide on 48000 and we get T=1000, so one tick=0,001sec)
* PC13
- GPIO_OUTPUT
