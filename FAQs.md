# Frequently Asked Questions

## Ubuntu Dual Boot -
**1.**  How much space you should give to Ubuntu while dual booting ? 

**Ans:** If you are dual booting Ubuntu only for this workshop, you can give around **100 GB** space. Allocate **30 GB** for **Root** ( / ), **8-10 GB** for **swap** area, remaining for **Home**. <br />
If you are planning to use Ubuntu furthur, dedicate **full D ( E or F )** drive to it ( **300 GB** in most of the cases ). Give **30 GB** for **Root**, **10 GB** for **swap** area, reamining for **Home**.

## ROS Installation

**1.**  I am getting the following error message after running ```sudo apt update```. What to do ?

<img src="W0_Images/PubKey.jpeg" width=700 height=150>

**Ans:**  Refer to the methods in this [link](https://answers.ros.org/question/325039/apt-update-fails-cannot-install-pkgs-key-not-working/) and hopefully the issue should be resolved.

<br/>

**2.**  I am getting the following error message after running ```sudo apt install ros-noetic-desktop-full```. What to do ?

<img src="W0_Images/apt_get_update.jpeg" width=700 height=300>

**Ans:**  Run ```sudo apt-get update``` and WAIT ! It takes time for this step to completely finish and it might seem like nothing is happening. Be patient.

<br/>

**3.** I am getting the following error message. What to do ?

<img src="W0_Images/Free_space.jpeg" width=800 height=50>

**Ans:** Refer to the methods in this [link](https://askubuntu.com/questions/178909/not-enough-space-in-var-cache-apt-archives) and hopefully the issue should be resolved.

**4.** I am getting the following error message after running ```sudo apt install ros-noetic-desktop-full```. What to do ?

<img src="W0_Images/Broken_package.jpeg" width=700 height=250>

**Ans:** TBD

**5.** I got like 'no valid openPGP data found'

<img src="W0_Images/pgp.jpeg" width=640 height=360>

**Ans:** run ```sudo apt-get install ca-certificates```

If that also doesn't work,try either

```
sudo apt-key del 421C365BD9FF1F717815A3895523BAEEB01FA116
#or
sudo -E apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```
