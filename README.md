# LineageOS-Switch-T210-UNOFFICIAL - Lineage OS 18.1 for Nintendo Switch
Unofficial Builds for LineageOS for the Nintendo Switch

## NOTE

Right now OTA Support is broken. I'll fix that later and publish a new release where it hopefully works. 


# Index
<b><a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL#lineageos-switch">LineageOS</a></b>

<b><a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL#lineageos-181-builds">LineageOS 18.1 Builds</a></b>

<b><a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL#how-to-flash-this-rom">How to flash this ROM</a></b>

<b><a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL#how-to-fix-bluetooth-keeps-stopping">How to fix "Bluetooth keeps stopping"</a></b>

<br/>


<br/>

# LineageOS Switch
<img src="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL/blob/cbbd7beacf2d2dabe3a01048806054a4c37ab069/pictures/switch_builds.png">
Android 11.x builds for Nintendo Switch based on the open-source project LineageOS
<br/>

All the builds in this repository are built using the official <a href="https://github.com/LineageOS/android">LineageOS</a> and <a href="https://gitlab.com/switchroot/android">Switchroot</a> sources

### Please read the disclaimer before you continue

```

Disclaimer from https://wiki.switchroot.org/en/Android/Build-11#:~:text=We%20highly%20recommend,all%20kernel%20files

Android 11 is not ready for release or for public usage. The source trees may
have missing bits or be incomplete, and issues will be present until the final
release. If you'd like to test Android 11 builds, you can ask to be a tester on
the Switchroot Discord server here: https://discord.com/invite/N9PPYXjWMY.

PSA and Licensing

LineageOS 18.1/Android 11/R for the Switch is an early work in progress. Do not
expect support or help or even a functional product. Please do not follow this
guide unless you have been directed to test 11 building by a Switchroot developer
or plan to contribute in some way--just use 10 as it is stable and more fully-featured.
Uploading repo copies without the original git history or unofficial builds without
credit is a violation of the Apache License, version 2.0, for all AOSP, LineageOS Project,
and Switchroot (via personal copyright) copyright-labelled files. The Linux kernel is
licensed under the GNU General Public License, version 2, and the same requirement for
history and/or credit applies to all kernel files.

If you want to be sure that everything works, take a LineageOS 17.1 Build from here https://download.switchroot.org/android-10/

```



```
#
# Copyright (C) 2016-2022 The LineageOS Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```


<br/>

All the builds in this repository are built using the official <a href="https://github.com/LineageOS/android">LineageOS</a> and <a href="https://gitlab.com/switchroot/android">Switchroot</a> sources

```
#
# Copyright (C) 2016-2021 The LineageOS Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```
## LineageOS 18.1 Builds

| Date   | LineageOS + NVIDIA                                   |androidTV + NVIDIA         |
| ------------------- | -------------------------------------------|-------------------|
| 20220713| <a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL/releases/tag/20220713.tab">Download</a> |<a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL/releases/tag/20220713.atv">Download</a> |

<br/>


# How to flash this ROM

```
NOTE: First follow [this]() before continuing!
```

1.- Grab the latest update from <a href="https://github.com/s3tupw1zard/LineageOS-Switch-T210-UNOFFICIAL/releases">Releases</a>
  (Download both files, the <b>lineage-18.1-[date]-[codename]-s3tupw1zard.zip</b> and the <b>sd_[date].zip</b>)
  
2.- Extract the <b>sd_[date].zip</b> contents into your SD Card root and copy the <b>lineage-18.1-[date]-UNOFFICIAL-[codename]-s3tupw1zard.zip</b> file in the root as well.
  
3.- Launch Hekate on your non-mariko Switch and go to <b>Tools> Arch bit • RCM • Touch • Partitions> Partition SD Card</b>

4.- Use the slider to give <b>Android</b> some space, then select <b>Next Step</b> to start the repartition process.

``` If hekate doesn't give you the chance to backup the SD files, repeat step 1 with the result partition scheme to copy the files in the main partition```
  
5.- Select the <b>Flash Android</b> option, when finished presh <b>Continue</b>.
  
6.- When prompted to reboot into TWRP, select <b>Continue</b>.
  
7.- In TWRP, select the <b>MOUNT</b> option and mount all possible partitions.

8.- Return to TWRP main menu and select the <b> Install </b> option , then <b>Select Storage</b> and choose the <b>Micro SD card</b> option and select the <b>lineage-18.1-[date]-UNOFFICIAL-[codename]-s3tupw1zard.zip</b> file from root directory.
  
  ```
  NOTE: Switch AArch is ARM64-v8a, choose ARM64 GApps package.
  
  NOTE: Download the matching OpenGAPPS-Package for Android 11 ONLY, others will not work
  
  - For the Tab version download the OpenGapps-pico Package
  
  - For the ATV version download the OpenGapps-tvmini package
  
  ```
  
  [OpenGapps](https://opengapps.org/)
  
  - Grab your downloaded OpenGAPPS package and put it on your sdcard root next to the lineage zip file
  
  - Choose the OpenGAPPS Package and swipe right to flash the file.
  
9.- Wait for the flash process to finish, then return and select <b>Reboot> System</b>.
 
10.- Your Switch will boot into LineageOS system with installed OpenGAPPS.


# How to fix "Bluetooth keeps stopping"
(Fix from this [issue](https://github.com/daviiid99/LineageOS-Switch-T210-UNOFFICIAL/issues/19)) - Thanks to @Marietuno from GitHub


1. Boot into Atmosphere OS (emuNAND/sysNAND) and pair a new joy-con set (this will write bluetooth MAC)

2. Reboot to hekate bootloader and select Nyx Options> Dump Joy-Con BT (this will dump 2 files to switchroot android folder called "joycon-mac")

3. Boot into TWRP and erase all partitions, flash the rom again and boot androidOS, bluetooth should be working now
