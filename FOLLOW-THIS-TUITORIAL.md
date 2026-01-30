# Linux-Phone-with-near-native-virtualization
You will be able to run Linux on your Android by following this guide. It does NOT need rooting and is EASY to setup with Termux

the reason I have created this GUIDE is there is no reliable way of running Linux ARM64 at near native speed on an Android Phone without ROOTING. As samsung removed that Option in OneUI 8, it drove me to make this project to help others like me. However, ANY ANDROID PHONE WILL WORK.

1. INSTALL THE PREREQUISITES
     -Install Termux from F-Droid (or the Google Play Store if you prefer it)
     -Install RealVNC viewer from your favorite app store (I installed it from the Play Store for reliable updates)
     -Make Sure your phone has at least 30GB of storage to be safe

2. IN TERMUX
   -pkg update && pkg upgrade
   -pkg install proot-distro
   *This makes sure that the necessary packages are installed for the coming steps

3. Install Distro of choice (Arch is not supported in this guide but you can try it if you're confident)
   - ex. proot-distro install ubuntu

4. Login to Distro
   -proot-distro login ubuntu

5. AFTER LOGIN
   -apt update && apt upgrade
   -apt install sudo nano wget curl htop

6. Install a Lightweight Desktop
   -apt install xfce4 xfce4-goodies

7. Install VNC Server
   - apt install tigervnc-standalone-server
   - To start VNCSERVER: vncserver
   - Enter password of your choice when prompted (you will have to remember this when you login to your machine from RealVNC)

8. Install RealVNC viewer on Android (https://play.google.com/store/apps/details?id=com.realvnc.viewer.android&hl=en_US&pli=1)

9. connect to localhost:5901 and BOOM! You should be in the desktop

    *IF YOU FOLLOWED EVERYTHING IN THIS GUIDE IT SHOULD'VE WORKED WITHOUT A PROBLEM, FEEL FREE TO CONTACT ME IF ANY PROBLEMS ARISE IN THE PROCESS OR IF THERE ARE ANY ERRORS IN THIS GUIDE😀
   * THIS GUIDE IS BEST OPTIMISED FOR DEBIAN BASED DISTROS 😀
   


   
   
    
   
   
     
