## `spi.c`

#### `void init_SPI(void)`

Description - initializes spi

* Switches off all other devices and initalizes spi(master)









## `uart.c`

#### `void init_UART0(void )`
Description - initialiaes one of the two uart channels
* 8 - bit data, 2 stop bits, baud rate = 9600

#### `void transmit_string_UART0(char *buffer)`
Description - transmits a string from uart0 channel





## `mag.c`

#### `void init_UART_MM(void )`

Description - Initializes the uart channel connecting the mc to the magnetometer




## `peripherals.c`

#### `void configure_torquer(void)`

Description - configures the input, output and the pwm pins (not clear how this works)





## `main.c`

#### `void TWI_init_master(void)`

Description - Initializes TWI and sets baud rate








## `timer.c`

#### `void timer_reset_two_sec(void)`
Clears the flags and resets the counter - **not too clear about this function**

## `common.h`
#### `define sbi(x,y)   (x |= (1<<y))`

## `xyz.c`
#### `void TWI_start(void)`
Initializes TWI transmission
* Transmits start condition and enables TWI
* Waits for acknowledgement

#### `void TWI_write_address(unsigned char data)`
Sends Slave addrss for TWI
* Sends address and data (direction)
* Waits for acknowledgement

#### `TWI_write_data(write_data)`
Function for master to write data into slave

#### `TWI_stop()`
Functtion to stop TWI
