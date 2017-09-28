* not clear about what is happening in (`peripherals.c - configure_torquer`) - something to do with pwm, but not clear how it is working and stuff

* (Resolved) What is CC1020 - it is switched off in SPI_Init  - Not used anymore - Ignore

* (Resolved) in main (beginning) what is this  (`Current_state.gps.gps_OC = 0;` )  ? Where is it initialized?  
    -  it is the struct that contains the data regarding the current state of the system. It is defined on peripherals.h
* (Resolved) What does `sei()` do in `xyz.c` ?  - It says that it switches on global interrupts - It is an avr function that is used to initialize avr interrupts
*  struct state is defined in peripherals.h, when it is declared in xyz.c, why aren't we prefixing an extern?
*  How is equinox defined?
* (Resolved)  Not too sure how the `sbi()` function is working - timer.c line 15 - it is defined in `common.h`
* what exactly does `write_data` do?
* `xyz.c` line 218 - how is PB5 being used as slave select
* Physical significance of `SS_GAIN` - defined in `quest.h`