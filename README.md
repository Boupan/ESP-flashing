# ESP-flashing
 ESPtool utilities

Standard procedure
'''
1)-pip install esptool
2)esptool.py --port com8 chip_id
3)esptool.py --port com8 flash_id
4)ONLY for newly bought v3 nodeMCU -> delete initial code 
  esptool.py --port com8 read_flash 0 0x400000 nodemcu_backup.bin
5)Filmware restore -> esptool.py --port com8 write_flash 0 nodemcu_backup.bin
'''
ALWAYS FLASH TWICE! bootloader


