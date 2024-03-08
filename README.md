# RicoLiveTD

RicoLiveTD is a lightweight tool to link Ableton Live with TouchDesigner through UDP and OSC.

## Installation

### Touchdesigner
Import the .tox into your project.
Open the parameters panel of the "RicoLiveTD" comp and set up the ports and ip address.
The data from Ableton Live flows out of the comp through its oulet as chop data.

### Ableton Live
There are three Max for Live objects. The first one (master) has to be put on the master bus. Set up there the IP address of the computer running TouchDesigner and the TouchDesigner UDP port (same as the one you set up in Touch Designer) and the Ableton Live listening UDP port.
The two others Max for Live objects (values and triggers) can be put on midi tracks and can transmit continuous datas (such as automations) and triggers (through midi notes).

#### Triggers
![alt text](Triggers.png?raw=true)
You can define up to 6 triggers and set the midi notes that trigger them.

#### Values
![alt text](Sliders.png?raw=true)

You can set up up to 4 parameter values per plugin instance. You can automate their slider and their name. Be sure to avoid duplicate parameter names through your Ableton session.
