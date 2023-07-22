# Wheel Speed Encoder
This C program is designed for the STM32 F103C8T6 and focuses on handling a wheel rotation sensor and transmitting the wheel speed over the Controller Area Network (CAN) communication protocol. The main function sets up the system clock, initializes GPIOs, and configures the CAN peripheral. An interrupt callback function HAL_GPIO_EXTI_Callback is used to calculate the wheel speed based on the time interval between two consecutive rotations of the wheel which is done by using the intervals between the positive rising edges of the sensor. The wheel speed data is then transmitted over the CAN bus using HAL_CAN_AddTxMessage in an infinite loop, with a 1-second delay between transmissions.

![image](https://github.com/ahmed23shaf/WheelSpeedEncoder/assets/112600024/552d0c4a-dcd3-48c8-8477-6e6faf631b4e)
![image](https://github.com/ahmed23shaf/WheelSpeedEncoder/assets/112600024/375038fc-10b5-4acd-b811-296abaa3f557)
