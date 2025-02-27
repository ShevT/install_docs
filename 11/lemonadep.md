### Pre-installation:

* **OOS 14 - 14.0.0.730(EX01) firmware is required** (from download page, firmware button)
* Optional gapps (from download page, gapps button)
* Optional KernelSU apk by **rsuntk** (get it on [release page](https://github.com/rsuntk/KernelSU/releases) from GitHub)


### First time installation (clean flash):

* Backup your data to PC, OTG flash drive
* Make sure you are on latest OOS 14
* Extract ***firmware flasher zip***
* Enter fastboot
* Execute ***Update-firmware.bat*** (windows) or ***Update-firmware.sh*** (Linux - make file executable) from extracted firmware flasher folder
* Now in recovery go to factory reset and confirm the reset
* Reboot to recovery
* Choose apply update and Apply from ADB
* Now install crDroid zip via sideload

```
adb sideload crDroid.zip
```
* When asked to sideload gapps, choose 'Yes' to reboot to recovery or 'No' if you don't want gapps and want to reboot to system
* Now if you choosed to install gapps, simply sideload gapps.zip the same way you installed crDroid.zip then reboot to system

### Update installation:
#### Firmware update (if needed):
* Extract ***firmware flasher zip***
* Enter fastboot
* Execute ***Update-firmware.bat*** (windows) or ***Update-firmware.sh*** (Linux - make file executable) from extracted firmware flasher folder (modem needs to be always updated, unless US variant)
* Proceed with below installation (via recovery)

#### Via recovery (recommended way):
* Boot to recovery
* Choose apply update and Apply from ADB
* Now install crDroid zip via sideload and reboot

```
adb sideload crDroid.zip
```
* If you had gapps, reboot to recovery and sideload gapps.zip and reboot

#### Via OTA:
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* If having gapps, reboot to recovery and sideload gapps package again
* Reboot