# rtl8723de
Realtek RTL8723DE module for Linux kernel

This device shows in lspci as "Realtek Semiconductor Co., Ltd. Device [10ec:d723]"

To install check terminal results for uname -r

 if your kernel is lower than 4.11,
 
sudo apt-get install build-essential git dkms

git clone -b 4.10-down https://github.com/jeremyb31/rtl8723de.git

sudo dkms add ./rtl8723de

sudo dkms install rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414

Then reboot

If you have kernel 4.11 and newer do

sudo apt-get install build-essential git dkms

git clone https://github.com/jeremyb31/rtl8723de.git

sudo dkms add ./rtl8723de

sudo dkms install rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414

Then reboot
