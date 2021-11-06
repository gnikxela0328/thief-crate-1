# thief-crate-1


This is The Thief Crate
<br />
 
<img src="https://github.com/gnikxela0328/thief-crate-1/blob/main/img/20211106_143502.jpg" />
<br />

A headless CDJ rig that comes complete with ssh/scp access and a c++ compiler (name another dj that...)
<br /><br />

# Why Thief Crate?
<br />
Thief Crate allows the user to have the full functionality of a pro CDJ setup at half the cost. The crate utilizes Mixxx, a free and open source dj software that is availble for Linux distributions (as well as other platforms). The controller is swappable, allowing the user to implement any MIDI device of their choice. In addition to sound control, the crate also leverages ubuntu's file system/networking capabilites to allow for wireless file transfer over local net. You can transfer files over most wireless networks (including a portable router or cellphone hotspot). 
<br />
File transfer can be performed WITHOUT interrupting the function of the crate for a seamless integration with the cloud.
<br />
<br />

# Parts List

<br />

<a href="https://www.raspberrypi.com/products/raspberry-pi-4-model-b/"> Pi 4 (8gb) </a>
<br />
<a href="https://amzn.to/3k8K5iM" > Screen </a>
<br />
<a href="https://www.sweetwater.com/store/detail/DDJSB3--pioneer-dj-ddj-sb3-4-deck-serato-dj-controller"> Controller </a>
<br />
<a href="https://www.sweetwater.com/store/detail/ScarSG3--focusrite-scarlett-solo-3rd-gen-usb-audio-interface"> Interface </a>
<br />
<br />

<img src="https://github.com/gnikxela0328/thief-crate-1/blob/main/img/20211106_143546.jpg" />

<br />

Some modification considerations:

<br />

The interface provides addtional input/output but can be easily replaced with a controller that has a soundcard compatible with Mixxx. Benefits include having an external volume control so you can more accurately dial in gain on the controller. 

<br />

The MIDI controller is swappable but requires you to configure the control surface in software (fairly easy)

<br /> 

The case is also optional. I built this wooden housing because I wanted a portable solution with a splash shield and a tabletop form factor.

<br /> 

Any computer can be used with this setup. I chose raspberry PI because of its compactness, one should note however, that a PI4 is necessary to run ubuntu.

<br />

For SSH acess, make sure to enable ssh-server on your target device
<br />

# Usage
<br />
Power it on like a normal computer and it is ready to go! 
<br />
<br />
If you wish to use the device wirelessly for file transfer (or other things) use nmap.

<br />
** Make sure you have permission to probe on your network 

<br />
<br />

First find the subnet your computer is on
```
ifconfig
```
For example network 192.168.1.0/24 :
<br />
On local computer (192.168.1.1)
```
sudo nmap 192.168.1.* -O
```
Your device will show up identified by its operating system


<img src="https://github.com/gnikxela0328/thief-crate-1/blob/main/img/20211106_144128.jpg" />

# Routing

<img src="https://github.com/gnikxela0328/thief-crate-1/blob/main/img/Untitled%20Diagram.drawio.png" />
