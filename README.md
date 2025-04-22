# USB-Relay-Lighting-Project
USB relay lighting project to automate home lighting
How to Control Your Room Lights Automatically Using a USB Relay and Your Home Theater Receiver
Overview
This DIY project will show you how to automate your room lighting using a USB-powered relay triggered by your AV receiver. When your receiver turns on, it powers a USB port, which in turn activates a relay to switch on a power strip connected to your room lights. This is a clean, reliable way to enhance your home theater or ambient lighting experience — no apps, no cloud, just pure automation.
My current configuration uses an iOS shortcut to wake Apple TV 15 seconds after connecting to the local network. When the Apple TV turns on it sends a CEC signal to an STR-DH-590 receiver to turn on. The receiver then outputs 5V 1A to a USB output on the back. This signal then trips a relay turning on a modified power strip to turn on room lighting.

What You'll Need
Components:
1x 5V Relay Module (single or dual channel)


1x USB cable (cut/stripped to expose terminals)


1x Power strip or extension cord (with black, white, green wires inside)


1x Project box or enclosure


14 AWG wire (for AC side)


Heat shrink tubing / electrical tape


Wire strippers, screwdriver, soldering iron (optional)
Tools (optional but recommended):
Multimeter


Hot glue gun

Wiring Instructions

 Single channel 5v relay. (Songle SRD-05VDC-SL-C) 
Step 1: Prep the USB Trigger
Cut a USB cable and strip the red (5V) and black (GND) wires.


Connect red to + (VCC) on the relay module. (Green wire in image below)


Connect black to both GND and S/IN (Purple wires in image below).




Step 2: Prepare the Power Strip
Cut the black wire (HOT) inside the extension cord.


Leave the white (Neutral) and green (Ground) wires intact.


Step 3: Wire the Relay (AC Side)
Connect the cut end from the wall to COM on the relay.


Connect the end going to the power strip to NO (Normally Open) on the relay.


When the relay is triggered by 5V USB, COM and NO close the circuit and power your strip.


Enclosure and Safety
Place your relay and wiring inside a plastic or non-conductive box.


Insulate all exposed wires with heat shrink tubing or electrical tape.


Use cable glands or rubber grommets where wires exit the box.


DO NOT daisy-chain power strips or exceed the relay's 10A/120V rating.

How It Works
Your device turns on.


The USB port outputs 5V power.


This powers the relay and activates it.


The relay closes the AC circuit to the power strip.


Room lights (or any device plugged in) turn on automatically.



Upgrades & Extensions
Add a second relay to control LED strips or fans.


Use a smart plug for remote override.


Integrate an ESP32 for Wi-Fi control or motion detection.


Add a Shortcuts automation on iPhone to wake the receiver when you arrive home.




Final Thoughts
This is a powerful little project that adds real convenience and ambiance to your space. Best of all, it's local, fast, and completely under your control.

