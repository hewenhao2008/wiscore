# WisCore SDK
<div align=center><img src="https://github.com/sevencheng798/wiscore/raw/master/img/inf_reg_wiscore.png"/></div>

![](https://github.com/sevencheng798/wiscore/raw/master/img/inf_reg_pic1.png)

This SDK is for WisCore hardware development platform base on OpenWrt system. Software features include three product series: WisAp, WisAvs(Amazon Alexa Avs function), WisGw(wiscore gateway)

Compiler introduction:<br>
If you are the first compiler SDK you need to choose to use the product type and then set the compiler environment. so that the next time you recompile the same types of products when there is no need to in the environmental settings unless you want to switch to other types of products

## For compiler WisAvs:
### Required Hardware
Before you get started, let's review what you'll need.<br>
1.WisCore development board -  Buy at Rakwireless - [wiscoreBoard](https://item.taobao.com/item.htm?spm=a1z10.5-c.w4002-14938546650.12.IKswLw&id=543868901011)<br> 
2.wisAudio board<br>
3.Micro-USB power cable<br>
4.Internet connection - Ethernet for download firmware to wiscore board<br>

### Let's get start to compiler wisAvs SDK
The original WisCore SDK on a wiscore board project required manual download and compile to run. To make the process faster and easier, we’ve included an compile install script with the project that will take care of all the heavy lifting. Not only does this reduce setup time to less than an hour on our wiscore board, it only requires developers to adjust three variables in a single install environment script - build/envsetup.sh 

#### Step 1: Clone the wiscore SDK
Open terminal, and type the following:<br>

    cd Desktop
    git clone https://github.com/sevencheng798/wiscore.git


#### Step 2: to set compile environment 
Before you run make, you need to set compile environment for the products you use with envsetup.sh, now we want to use the Amazon Alexa function so we should choose wisAvs products types. 

    cd ~/Desktop/wiscore
    ./build/envsetup.sh wisAvs hgw

#### Step 3: Run Make to compile
You are now ready to run make command to compile. This will install all dependencies, including to compile openwrt and related application

Note: Finally compiled generated files firmware in the folder out/target/bin

To run the make, open terminal and navigate to the folder where the project was cloned. Then run the following command:

    cd ~/Desktop/wiscore
    make

#### Step 4: burn the firmware to wiscore board
[How to burn firmware to WisCore Board](https://github.com/sevencheng798/wiscore/wiki/Burn-Firmware-for-WisCore-Board)<br> 
## For compiler WisAp:
### Required Hardware
Before you get started, let's review what you'll need.<br>
1.WisCore development board Buy at Rakwireless - [wiscoreBoard](https://item.taobao.com/item.htm?spm=a1z10.5-c.w4002-14938546650.12.IKswLw&id=543868901011)<br> 
2.Micro-USB power cable<br>
3.Internet connection - Ethernet for download firmware to wiscore board<br>

### Let's get start to compiler wisAp SDK
The original WisCore SDK on a wiscore board project required manual download and compile to run. To make the process faster and easier, we’ve included an compile install script with the project that will take care of all the heavy lifting. Not only does this reduce setup time to less than an hour on our wiscore board, it only requires developers to adjust three variables in a single install environment script - build/envsetup.sh 

#### Step 1: Clone the wiscore SDK
Open terminal, and type the following:<br>

    cd Desktop
    git clone https://github.com/sevencheng798/wiscore.git


#### Step 2: to set compile environment 
Before you run make, you need to set compile environment with envsetup.sh

    cd ~/Desktop/wiscore
    ./build/envsetup.sh wisAp hgw

#### Step 3: Run Make to compile
You are now ready to run make command to compile. This will install all dependencies, including to compile openwrt and related application

Note: Finally compiled generated files firmware in the folder out/target/bin

To run the make, open terminal and navigate to the folder where the project was cloned. Then run the following command:<br>

    cd ~/Desktop/wiscore
    make

#### Step 4:  burn the firmware to wiscore board
[How to burn firmware to WisCore Board](https://github.com/sevencheng798/wiscore/wiki/Burn-Firmware-for-WisCore-Board)<br>
## Please refer to the use of more detailed introduction
[get_quick_started_with_wiscore](https://github.com/sevencheng798/get_started_with_wiscore)

