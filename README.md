# ricolivetd

RicoLiveTD is a lightweight tool to link Ableton Live with TouchDesigner through UDP and OSC.

## Installation

### Touchdesigner
Import the .tox into your project.
Open the parameters of the "Rico Live TD" comp and set up the incoming UDP port.
All the data from ableton live go out of the comp (through its oulet) as chop data.

### Ableton Live
There are three max for live objects. The first one (master) has to be put on the master bus. Put in it the IP address of the computer running TouchDesigner and the TouchDesigner UDP port (same as the one you set up in Touch Designer).
The two others (values and triggers) can be put on midi tracks and can transmit continuous datas (such as automations) and triggers (through midi notes).
