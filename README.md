# Nucleo_L476RG_USART_RxTx_v1
STM32 polling_Tx interrupt_Rx
This project was developed on a Nucleo_L476RG board using the Low Level drivers library to drive the USART device.

GPIO and USART peripherals are configured to receive characters 
from an HyperTerminal (PC) in Asynchronous mode using an interrupt
USART Peripheral is configured in asynchronous mode (115200 bauds, 8 data bit, 1 start bit, 1 stop bit, no parity).

When character is received on USART Rx line, a RXNE interrupt occurs. 
USART IRQ Handler routine is then checking received character value. 
Each character is stored in a buffer until a carriage return character or line feed character is received.
The contents of the buffer are then displayed using a polling method.



