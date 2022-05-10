# DRC-SIM-BACKEND for `Windows Subsystem for Linux`
The original repository is needed for this to work. It can be found here: https://github.com/rolandoislas/drc-sim
I got the idea to try this from a discussion I had on reddit: https://www.reddit.com/r/WiiUHacks/comments/mp2htx/so_streaming_the_wii_u_to_a_pc_without_a_capture/guas5cj/?context=3

To use this you need to follow these steps:
## 0. Have any Linux Subsystem installed (WSL)

## 1. Install DRC-SIM
As you might have guessed you will need to have the app installed below your Linux Subsystem. To do this you will want to copy this command into the command line and execute it:
`curl -s https://raw.githubusercontent.com/rolandoislas/drc-sim/develop/install.sh | sudo bash -s develop`

You could also use the included shell script to handle the task for you.

Source (for future changes or issues): https://github.com/rolandoislas/drc-sim/wiki/Install-Script#easy-install

## 2. Install xMing
In this repository is a copy of the xMing installer for windows. Execute it and install xMing on your windows machine. If it is installed succesfully launch it and go to the logs.
The Ip should be listed under "XdmcpRegisterConnection:".

Source: https://sourceforge.net/projects/xming/

## 3. Export the Linux Display
In order to use xMing with Linux type `export DISPLAY=%ip%:0`into a Linux command line and replace %ip% with your Ip that you got from the xMing Logs.

## 4. Launch DRC-SIM
Now you are ready to launch drc-sim. Type `drc-sim-backend` into the Linux command line and check that there are no errors. If everything works you should see xMing open a small drc-sim control panel.

## Notes:
You can skip step 3 and 4 by launching the supplied shell file.

## Donations

If you enjoy my work, why not buy me a coffee?      
[![paypal](https://www.paypalobjects.com/en_US/DK/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/donate/?hosted_button_id=K5KVUTX6HJHXU)

Of course, if you choose to enjoy it for free, I also appreciate it.
