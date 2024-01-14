README - HotStart Challenger 650 TouchOSC Project v1.00

Author: Tyler Choo

This project includes files to use TouchOSC for iPadOS to control functions in the HotStart Challenger 650.

Please send any feature requests or report any bugs to n371tc@gmail.com.

--------------------------------------------------------------
# Version Notes

v1.00
	Initial Release

--------------------------------------------------------------
# Requirements

## Computer
- X-Plane 11/12
- HotStart Challenger 650 (Stable or Beta)
- TouchOSC Bridge (https://hexler.net/touchosc)
- XMidiCtrl (https://forums.x-plane.org/index.php?/files/file/76419-xmidictrl-a-midi-controller-plugin-for-x-plane/)

## iPad:
- TouchOSC (https://apps.apple.com/us/app/touchosc/id1569996730)

--------------------------------------------------------------
# Installation and Configuration

## Computer
	
1. Install the required applications and plugins (above).

2. Place XMidiCtrl.toml into "[X-Plane 12 Directory]/X-Aviation/CL650"

## iPad

1. Download the TouchOSC (Challenger.tosc) template and open it with the TouchOSC app to load it into the app. 

2. Launch TouchOSC and open the Challenger.tosc file.

3. Open the Connections menu (link symbol in the header).

4. Enable Bridge Connection 1 and select your computer running TouchOSC Bridge, or enter its local IP address.

5. Enable MIDI Connection 1.
	a. Set Send Port to <Bridge 1>.
	b. Set Receive Port to <Bridge 1>.

--------------------------------------------------------------
# Operation

1. Ensure TouchOSC Bridge is running on your computer.

2. Start X-Plane and start a flight in the HotStart Challenger 650.

3. Start TouchOSC on your iPad. Ensure the Challenger file is open. Click the Play button in the header.

4. You should now be able to control the Challenger with your iPad!

--------------------------------------------------------------
# Notes

1. The MIDI port configuration in "XMidiCtrl.toml" is set to 0 for both OUT and IN. This assumes you have no other MIDI devices connected to your computer. In case you do, adjust the port so that it matches the port for TouchOSC Bridge. Your port configuration can be viewed in X-Plane by going to Plugins -> XMidiCtrl -> Show MIDI Devices. For more XMidiCtrl help, consult their site: https://forums.x-plane.org/index.php?/files/file/76419-xmidictrl-a-midi-controller-plugin-for-x-plane/.

2. Most buttons will react to their actual in-aircraft state, but sliders do NOT. I am still working on a decent way to implement this.

3. Knob control was very finicky. The autopilot knobs have incremental controls in the TouchOSC template, but typically it is much faster to use your scroll wheel on your computer instead. 