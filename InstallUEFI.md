# Installing UEFI

![image](https://github.com/user-attachments/assets/003238ad-76bb-4132-be0e-bb6ddbf15c45)

- Connect your Pixel Watch 3 to your computer using the charging cradle that *shipped with it* (This is important, as it brings in USB support on your watch)

Note: below steps will erase all content on your watch.

- Unlock your watch bootloader by:
    - Go to settings on your watch
    - Open about
    - Tap 7 times (or so) on build number
    - Go to the newly appeared for developers section
    - Enable ADB USB Debugging
    - Enable OEM Unlock
    - Open a terminal on your computer
    - 🏃‍♂️ adb reboot bootloader
    - 🏃‍♂️ fastboot flashing unlock

- Re-enable ADB via settings after your watch is reset and erased
- 🏃‍♂️ adb reboot bootloader
- Download the UEFI image from the UEFI release page (https://github.com/WOA-Project/mu_seluna_platforms/releases/latest)
    - Pay attention to your watch model, use Luna for the big watches, and Selene for the small watches
- 🏃‍♂️ fastboot boot uefi.img
- Your watch should now show an old clock icon

![image](https://github.com/user-attachments/assets/9d630972-0434-4708-b5bb-9a0d8f82f9ab)

You did it!
