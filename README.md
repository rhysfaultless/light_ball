# light_ball

<br/>

<p align="center"><img src="/readme_assets/banner_v1.jpg" width="600"/></p>


## Background

Christmas lights on trees are beautiful, but the light strings are difficult to install.
It is possible to install lights in conifer trees using a ladder and pole.

<p align="center"><img src="/readme_assets/amazon_B0BN6MBTHW.jpg" width="300"/></p>

Example, _[Amazon B0BN6MBTHW](https://www.amazon.ca/Telescopic-Telescoping-Installation-Birdfeeders-Lightweight/dp/B0BN6MBTHW)_

This works when the tree is less than 10 metres tall _(35 feet)_, noting that it is difficult to remove the lights. 
Taller trees and deciduous trees require a boom-lift, due to the tree's height and limited access between branches.

<p align="center"><img src="/readme_assets/boom_lift.png" width="300"/></p>

Home Depot rents these boom-lifts:

| Height    | Height  | Rental cost, per day _(Canadian dollars, 2024)_ |
| :-------: | :-----: | :---------------------------------------------: |
| 10 metres | 35 feet | $370                                            |
| 15 metres | 50 feet | $490                                            |

It's a significant investment; especially if you plan to remove the lights after the season, or when you consider the maintenance task of replacing lights that burn out.


### Background, Light Options To Consider

| Light Option | Image                                        | Notes |
| :----------: | :------------------------------------------: | :---: |
| None         | ![](/readme_assets/tree_plain.png)           |       |
| Draped       | ![](/readme_assets/tree_lights_draped.png)   | String lights draped over the tree's canopy. This does not look good. |
| Spiral       | ![](/readme_assets/tree_lights_spiral.png)   | String lights wrapped around the tree's canopy. This looks good, but takes a long time to install. |
| Wrap         | ![](/readme_assets/tree_lights_wrap_v2.png)  | String lights wrapped around the tree's trunk and branches. This looks good, but takes a long time to install. |
| Vertical     | ![](/readme_assets/tree_lights_vertical.png) | String lights hanging from tree branches, similar to a weeping willow's hanging branches. |
| Balls        | ![](/readme_assets/tree_lights_balls.png)    | There are consumer options available, with single colours, and up to 300 mm diameter. There are larger options, but they are intended for use on the ground since they are heavy or have high wind resistance. |
| Flood        | ![](/readme_assets/tree_lights_flood.png)    | Inexpensive light at the base of the tree. Typically floods the tree with a single colour of light, with minimal range. It can get covered from snowfall. |
| Laser        | ![](/readme_assets/tree_lights_laser.png)    | Inexpensive light at the base of the tree. It makes many small dots on the tree, but also has a long overshoot onto surfaces behind the tree. It can get covered from snowfall. |


### Background, Power Sources For Lights

* AC mains power, as how most North American christmas lights are powered.
* Low voltage DC cable run up the tree. 12 VDC custom outdoor wiring does not require inspection from Electrical Safety Authority in Ontario Canada. 
* Wireless power transimission, such as Disney's: _[Wireless Power Transmission Safely Charges Devices Anywhere Within A Room](https://la.disneyresearch.com/innovations/wireless-power-room/)_.
* Solar panels on the lights, with a battery.
* PoE _Power Over Ethernet_. The passive option uses 24 VDC, the active options use 48 - 52 VDC.


### Background, Installation Methods To Consider

1. Ladder and pole.
2. Pole with a hook.
3. Pole with a catch release.
4. Climbing trees.
5. Drone with a catch release
6. Lights installed onto a drone. The drone would remain in the tree.
7. Pulleys installed into trees, which then allow the lights to be raised and lowered. This is similar to a flag pole.


### Background, Design Requirements

1. Colours and white available _(preferably user selectable after installation)_
2. Lights visible at dusk.
3. DC low voltage, or existing approved device.
4. IP54 minimum, to allow for rain and snow melt.
5. Approved FCC or Industry Canada components to not cause RF issues. This is only relevant if the devices include Wi-Fi, Bluetooth, Zigbee, or similar radio communication.


### Background, Design Intent

There is an unmet design space for Light Balls and Vertical Strands that can be installed in tall trees.
It is uncommon to see Spiral or Wrapped string lights on tall trees due to the installation cost.
People sometimes add Flood or Laser lights, but the light concentrates near the base of the tree.
The goal is to design a light source that:

1. Can be installed in a large tree using methods such as a ladder-and-pole, a boom-lift, or using a drone _(preferred option)_. 
2. Can be powered from this location. Any safe power method is acceptable, but it should consider installation difficulty, maintenance burden, and reliability.


## Concept 2024-12

<p align="center"><img src="/readme_assets/concept_sketch_construction.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/ball_construction_far.jpg" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/ball_construction_close.jpg" width="300"/></p>

### Concept 2024-12, Parts List

| Subsection   | Description                                | Vendor        | Item                                                       |
| :----------- | :----------------------------------------- | :------------ | :--------------------------------------------------------- |
|              |                                            |               |                                                            |
| Frame        | 14 AWG galvanized steel wire _(Ø2 mm)_     | Home Depot    | 1001028009                                                 |
| Frame        | 24 AWG galvanized steel wire _(Ø0.6 mm)_   | Home Depot    | 1001027858                                                 |
| Frame        | Cyanoacrylate                              | Loctite       | 401                                                        |
|              |                                            |               |                                                            |
| Electronics  | ESP32 microcontroller                      | Amazon        | B0D8T7Z1P5                                                 |
| Electronics  | DC-DC buck converter                       | Amazon        | B07V4RT4H8                                                 |
| Electronics  | Light Strands, WS2812B                     | Amazon        | B0CD1YBFPX                                                 |
| Electronics  | Solder                                     |               |                                                            |
| Electronics  | Flux for soldering                         |               |                                                            |
| Electronics  | Hook-Up-Wire, 20 AWG, Red                  |               |                                                            |
| Electronics  | Hook-Up-Wire, 20 AWG, Black                |               |                                                            |
| Electronics  | Hook-Up-Wire, 20 AWG, Yellow               |               |                                                            |
| Electronics  | Fuse 3 A                                   | Digikey       | F2583CT-ND                                                 |
| Electronics  | M12 bulkhead connector, 5-position, female | Digikey       | A126843-ND                                                 |
| Electonics   | Enclosure body                             | Custom        | [enclosure_body.stl](./enclosure_files/enclosure_body.stl) |
| Electronics  | Enclosure lid                              | Custom        | [enclosure_lid.stl](./enclosure_files/enclosure_lid.stl)   |
|              |                                            |               |                                                            |
| Power Supply | Power supply, 110 VAC to 12 VDC, 5 A       |               | _recovered from e-waste_                                   | 
| Power Supply | Fuse, ATO, 3 A                             | Digikey       | F4193-ND                                                   |
| Power Supply | Fuse holder                                | Digikey       | FHAC0001ZXJA-ND                                            |
| Power Supply | Terminal block, 6-position, Red            | Digikey       | 277-15998-ND                                               |
| Power Supply | Terminal block, 6-position, Black          | Digikey       | 277-15783-ND                                               |
| Power Supply | Terminal block, 6-position, Brown          | Digikey       | 277-18255-ND                                               |
| Power Supply | Cable, 2X 20 AWG                           |               |                                                            |
| Power Supply | M12 inline connector, 5-position, male     | Digikey       | A133885-ND                                                 |
| Power Supply | Waterproof box                             | Canadian Tire | EF-B02                                                     |
| Power Supply | AC extension cable                         |               |                                                            |
|              |                                            |               |                                                            |
| Network      | 2.4 GHz access point / router              |               |                                                            |


### Concept 2024-12, Frame

The ball has 3 vertical metal hoops, and a spiral of metal wire around the hoops.
These main structural pieces use galvanized 14 gauge steel wire _(Ø2 mm)_.
The structural pieces are tied together using short sections of galvanized 24 gauge steel wire _(Ø0.6 mm)_.
These tied joints are then coated with cyanoacrylate _(Super Glue)_.
I then added a hook to the ball, using the same 14 gauge wire.
There is a section of rubber heat-shrink-tube on the hook, to minimize abrasion to the tree's bark.

_Notes:_ 
* _The hook should use thicker material in future iterations, as it was prone to bending during installation in the tree._ 
* _It took a long time to make these balls. Consider using a 3D printed ball, or developing tooling to tie to metal hoops together._


### Concept 2024-12, Electronics Soldering

<p align="center"><img src="/readme_assets/concept_sketch_controller.png" width="600"/></p>
<br/>
<p align="center"><img src="/readme_assets/wiring_diagram_2024-12.png" width="600"/></p>
<br/>

The wiring diagram above shows the electronics for the Light Ball.
I soldered these components together.

_Note that I did not include a level converter for the light's data line._
_The ESP32 outputs 3.3 V on its D13 line, but the lights suggest an input signal of 5 V._
_I did not include a level converter, since my lighting test results seemed acceptable, without unintended colours of flickering._


### Concept 2024-12, Electronics Firmware And Configuration

With the electronics soldered, I then connected the ESP32 development board to my computer with a USB cable.
I went to [install.wled.me](https://install.wled.me/), selected firmware version 0.14.4, and then clicked install.
In the pop-up window, I selected the relevant computer port.

<p align="center"><img src="/readme_assets/wled_firmware_installation.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_flashing_in_progress.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_flashing_complete.png" width="300"/></p>
<br/>

After installing the firmware, the WLED installer will ask you to enter Wi-Fi network details.

<p align="center"><img src="/readme_assets/wled_network_scan_in_progress.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_network_details.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_network_complete.png" width="300"/></p>
<br/>

You can click _Visit Device_, which will navigate to the ESP32's webpage.
_Note: I had to first switch my computer to a new Wi-Fi SSID, since I am using a separate LAN network without internet access to simplify security._

<p align="center"><img src="/readme_assets/wled_configuration_home.png" width="300"/></p>
<br/>

_The browser's URL is a dyanmic address that my router assigned._
_I will change this to a Static IP in a later section of this readme._

Next, I clicked the gear in the top right corner to configure:

* LED Preferences
  * GPIO as pin D13
  * Length as the number of WS2812 LEDs in the string
* Sync
  * The primary ESP32 ball as the Leader
  * Other ESP32 light balls as the Followers
  * _Sync will have all the light balls follow the same light patterns_
* Time & Macros
  * _Setting times when the lights change patterns._
  * _This is only required on the Leader._
  * _Followers should also have the OFF settings, incase they lose Wi-Fi connection._
  * _Preset 0 is set to black, to shut the lights off._
  * _Preset 1 is set the colour pattern I want to use._

<p align="center"><img src="/readme_assets/wled_configuration_settings.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_configuration_led.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_configuration_sync_leader.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_configuration_sync_follower.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_configuration_time.png" width="300"/></p>
<br/>
<p align="center"><img src="/readme_assets/wled_configuration_time_controlled_presets.png" width="300"/></p>
<br/>


