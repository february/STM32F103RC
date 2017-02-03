启动OPEN OCD服务
sudo openocd -f /usr/share/openocd/scripts/interface/stlink-v2.cfg -f /usr/share/openocd/scripts/target/stm32f1x.cfg

启动GDB TUI
sudo arm-none-eabi-gdb -tui miniblink.elf

从GDB连接OPEN OCD
target remote localhost:3333