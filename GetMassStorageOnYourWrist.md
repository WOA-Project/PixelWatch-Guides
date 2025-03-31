# Mass Storage

Watches being advanced alien technology, you can get them into mass storage, yes.

Here is how:

- Download the [bootpkg](/bootpkg.bin)
- 🏃‍♂️ adb reboot bootloader
- 🏃‍♂️ fastboot getvar current-slot
    - if above says a:
        - fastboot flash modem_b bootpkg.bin
    - if above says b:
        - fastboot flash modem_a bootpkg.bin
- 🏃‍♂️ fastboot boot uefi.img

![image](https://github.com/user-attachments/assets/1a846af8-375b-4af8-86b5-8b4498d6cfa9)

- Admire the very fitting boot menu ui, and press the digital crown to enter that option

![image](https://github.com/user-attachments/assets/5f929f74-3992-45b7-aac5-62202d1e5dea)
_Alignement, check!_

- You are now in mass storage, it may be a good time to actually backup your watch before you screw something up, for real.

![image](https://github.com/user-attachments/assets/b390ae49-d318-4ef8-89d5-31de2123308c)
![image](https://github.com/user-attachments/assets/7511c92b-e321-42ec-a005-777c619a0bf3)


To revert the boot menu install:

- 🏃‍♂️ adb reboot bootloader
- 🏃‍♂️ fastboot getvar current-slot
    - if above says a:
        - fastboot erase modem_b
    - if above says b:
        - fastboot erase modem_a

Thats it!
