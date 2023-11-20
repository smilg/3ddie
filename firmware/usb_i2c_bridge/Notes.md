# I/O Pin Setup
|Name     |GPIO #|Pkg #|Config        |
|:-------:|:----:|:---:|:------------:|
|MCLR     |29    |41   |Out PU        |
|TS (EIO0)|14    |17   |In/Out        |
|SDA (SI0)|12    |15   |I2C_SDA (i2c0)|
|SCL (SI1)|13    |16   |I2C_SCL (i2c0)|

# rp2040 i2c interface notes
## functions
### int main(void): setup stuff
* call board_init() - pico SDK function
* call tusb_init() - for tinyusb stuff
* set gpio pin modes, initialize i2c
* infinite loop tud_task() - for tinyusb

### void tud_mount_cb(void): invoked when device is mounted
* empty

### void tud_umount_cb(void): invoked when device is unmounted
* empty

### void tud_suspend_cb(bool remote_wakeup_en): invoked when usb bus is suspended
* empty

### void tud_resume_cb(void): invoked when usb bus is resumed
* empty


# gestic.c notes