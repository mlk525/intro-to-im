# Production Assignment: Analog + Digital LED Control

## Description
Reading information received from a potentiometer as well as a momentary push button, four LEDs are controlled based on this input. The LEDs will blink one and off no matter what, but the push button controls the pattern in which they blink, and the potentiometer control the time interval of each blink.
<p align="center">
  <br>
  <img width="700" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%2016%20(arduino%20io)/pictures/Aesthetic.jpg">
</p>

Using the basic analogRead(), digitalRead() and digitalWrite() functions, we achieve the desired operating style. This design was partially inspired by button-controlled bike lights. the time interval was controlled by changing the value inside the delay() function, and the alternating effect was achieved by reversing the value assigned to the ledState (ledState = !ledState) at the start of each iteration.

### Circuit Schematic:

<p align="center">
  <br>
  <img width="700" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%2016%20(arduino%20io)/pictures/test_schem.png">
</p>

### Project Photographs:

Front View
<p align="center">
  <br>
  <img width="700" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%2016%20(arduino%20io)/pictures/Front.jpg">
</p>

Top View
<p align="center">
  <br>
  <img width="700" src="https://github.com/mike-leo-k/intro-to-im/blob/master/june%2016%20(arduino%20io)/pictures/Aerial.jpg">
</p>

## Challenges & Discoveries
* 