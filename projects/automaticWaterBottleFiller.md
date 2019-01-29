---
layout: project
type: project
image: images/arduino.jpg
title: Automatic Water Bottle Filler
permalink: projects/automaticWaterBottleFiller
# All dates must be YYYY-MM-DD format!
date: 2016-12-07
labels:
  - C
  - Arduino
  - RFID
summary: A water bottle refiller that remembers container sizes.
---

<img class="ui image" src="{{ site.baseurl }}/images/arduino.jpg">

My partner and I proposed,designed and constructed a device that would automatically fill a container based on a stored size so that the user would not have to stand at the water station the entire time.

## Problem
I noticed that I was spending valuable minutes out of my day filling up my 40 oz hydroflask. In fact I was spending about 1 minute every day during the most valuable time in the morning when I am getting ready for my day. So I thought there must be a way to press a button and fill up my water bottle without having to stand there to fill it up.

## Ideas
My partner and I thought about ways to recognize containers and came up with ultrasonic sensors and RFID chips. After some research the ultrasonics proved to be more unreliable at close range and would require more calibration than we had time for, so we decided to use RFID chips.

Next was a method of dispensing the water. This was either a valve to allow flow of water, or a pump to pump the water through a hose. Initially we thought a valve would be easier on power so we tried this option. Upon first prototype we discovered that the valve we were using required a certain pressure to allow proper flow. We then moved to purchase a small pump to fix this problem, verifying the power and flow specifications more carefully before deciding this time.

## Final Product
The device scans a RFID chip, programs the value of the chip with the duration you fill the container of water, then when you fill it up again, you could scan it and press one button to dispense automatically.

This was based on the Arduino Uno connected to a custom circuit to power the pump and a RFID reader to read the chips. We used a pet food container to store the water and a flexible plastic hose connected to the pump to dispense the water. The circuit was connected to the Arduino.

## Expandability
While we used RFID chips separate from containers, this could be manufactured into sleeves or smaller patches to go onto water bottles more conveniently, allowing the user to just place the water bottle and not worry about scanning a chip. This technology could also be integrated into refrigerators or other water stations already on the market at a relatively low cost.

You can see a demonstration of the final product on [YouTube](https://www.youtube.com/watch?v=wDVQtC7__SE).
