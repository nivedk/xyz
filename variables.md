* state Current_state - A structure that contains a lot of data from MM, SS, GPS etc. 
    - Defined in peripherals.h
    - Instance Current_state created in xyz.c
* extern uint_64 Time - Stores the time in seconds since equinox - (not clear how equinox is defined)
    - Defined in peripherals.h
* extern uint8_t Mode - Stores mode of the satellite PREFLIGHT, NOMINAL, SAFE, EMERGENCY, DETUMBLING
    - Defined in peripherals.h
* unsigned char write_data - Stores data to be written by master into slave - done once every iteration (TWI_Write)
    - Defined in xyz.c