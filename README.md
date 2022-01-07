# zmk-config
Download The Archive

Once the setup script is complete and the new user config repository has been pushed, GitHub will automatically run the action to build your keyboard firmware files. You can view the actions by clicking on the "Actions" tab on your GitHub repository.

![Actions](https://zmk.dev/assets/images/github-actions-link-eabc7686fe9b218d6ac8349601b684fa.png)



Once you have loaded the Actions tab, select the top build from the list. Once you load it, the right side panel will include a link to download the firmware upload:

![Artifacts](https://zmk.dev/assets/images/firmware-archive-d6e735a9fc2ab0463ea0f1f9e0b6de3c.png)


Once downloaded, extract the zip and you can verify it should contain one or more uf2 files, which will be copied to your keyboard.

Flashing UF2 Files

To flash the firmware, first put your board into bootloader mode by double clicking the reset button (either on the MCU board itself, or the one that is part of your keyboard). The controller should appear in your OS as a new USB storage device.

Once this happens, copy the correct UF2 file (e.g. left or right if working on a split), and paste it onto the root of that USB mass storage device. Once the flash is complete, the controller should automatically restart, and load your newly flashed firmware.
