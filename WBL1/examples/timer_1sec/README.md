This example initiliases TIMER 2 of WillowBee with 1000 millisecond interrupt and it print out the seconds as follows:

<img src="https://willowsoft.co/wp-content/uploads/timer_1sec.jpg" width=60% height=60%>

To edit interrupt content edit the TIM2_IRQHandler function that is defined in the following file.
C:\bipom\devtools\WillowBee\WBL1\examples\timer_1sec\Core\Src\stm32wlxx_hal_msp.c


void TIM2_IRQHandler(void)
{
  /* USER CODE BEGIN TIM2_IRQn 0 */
  HAL_TIM_IRQHandler(&htim2);
  /* USER CODE BEGIN TIM2_IRQn 1 */
  /* USER CODE END TIM2_IRQn 1 */
}



