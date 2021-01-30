# AR3 Hardware Mods
Some modifications that I've made to the AR3 hardware. They are designed to be added on with minimal disassembly.

## Joint Position Encoders
The original rotor encoder design provides good resolution and, despite backlash and other sources of inaccuracy, works well for applications that only require repeatability. Task positions can be taught and the actual joint positions do not matter too much. However, goals produced by motion planning require accurate correspondence between the actual and intended positions of the arm. At the cost of some resolution, we can achieve much more accurate control of the arm with joint position encoders. With the AMT-102V encoders at the maximum 2048 pulses per revolution, we can get 8192 counts with quadrature decoding, giving us a respectable resolution of 0.05 degrees per encoder count which is acceptable given that there are probably other more significant sources of error.

I've managed to get joint encoders set up for J2 and J5. I intend to move the J5 limit switch to calibrate with the J6 housing directly, as having it calibrate against the belt carrier still leaves some room for error. I am working on J3 as well, though I'm having more issues with slipping on the motor shaft instead so I'll try to get that resolved first.

-----

### J2 Joint Encoder
* The spindle adapter can be screwed over the existing J2 drive spindle, replacing every other screw. You'll need longer M3 flathead screws.
* Glue the two parts of the assembly together
* The entire piece will snap on the the J2 turret housing

  <img src=./images/j2_assembly_1.jpg width="200">
  <img src=./images/j2_assembly_2.jpg width="200">
  <img src=./images/j2_assembly_3.jpg width="200">

-----

### J5 Joint Encoder
* You can just glue the extension on to the J6 housing
* You'll want to use the longer M3 screws for the covers to secure the adapter
* I chose to leave the wires outside but with a little more effort you could squeeze them into the cover spacer and make everything a little neater.

  <img src=./images/j5_cover.jpg width="200">

-----