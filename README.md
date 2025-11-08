# SimpleSwitch

![Render of SimpleSwitch](https://github.com/miket6000/SimpleSwitch/blob/main/docs/SimpleSwitch.png?raw=true)

SimpleSwitch is a magneticly operated electronic switch designed for model rocketry. It is a 15x10mm PCB with an input and output capable of switching approximately 4A continuous and 10A for 10s.

It is designed specifically to be easy to turn on, but to require multiple steps to turn off. This is to prevent issues with accidental turn off which can occur with traditional magnetic switches when they pass by magnatized hardware on launch towers/rails.

The magnetic switch draws a very small amount of power from the battery when plugged in. This is calculated at 3uA worst case, so a small 150mAh 1s battery should last approximately 5 years. On larger batteries this is quickly swamped by the batteries self discharge rate.

## Operation

Use of the SimpleSwitch is easy. Bringing a magnetic south pole near the top of the board will result in the switch turning on and illuminating both the red and green LEDs, the switch is now in the "ON" state. 

To turn off the switch you nead to put a North pole near the switch which will cause the red LED to turn off ("OK" state). Bringing a South pole near the switch will then cause the green LED to turn off and the red LED to turn back on ("WARNING" State). One more north pole will cause the red LED to turn off and the switch to disable the output ("OFF" State).

In summary as you alernate South-\>North-\>South-\>North you step through the states as shown below:

| State Name  | Red LED | Green LED | Switch State |
|-------------|---------|-----------|--------------|
| OFF         | OFF     | OFF       | OFF          |
| ON          | ON      | ON        | ON           |
| OK          | OFF     | ON        | ON           |
| WARNING     | ON      | OFF       | ON           |
| OFF         | OFF     | OFF       | OFF          |
