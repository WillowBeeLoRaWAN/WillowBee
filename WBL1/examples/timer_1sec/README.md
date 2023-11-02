> [!NOTE]
> This example initiates TIMER 2 of WillowBee with a 1000 millisecond interrupt, and it prints out the seconds as follows:

<img src="https://willowsoft.co/wp-content/uploads/timer_1sec.jpg" width=60% height=60%>

To edit interrupt content, edit the **TIM2_IRQHandler** function that is defined in the following file:
**C:\bipom\devtools\WillowBee\WBL1\examples\timer_1sec\Core\Src\stm32wlxx_hal_msp.c**


> [!IMPORTANT]
> This example uses a 48 MHZ clock configuration for the timer interrupt. If the code copies another system that runs at a different clock speed, then the prescaler and counter period should be set according to the timer interrupt time.


