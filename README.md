# GPS-Guided Rocket Glider

## Overview

I want to build a GPS guided R/G (rocket glider). A rocket glider is a model rocket that goes up as a model rocket and glides down in one piece as a glider. The problem is, if the model goes too high, the glider can drift away and cannot be recovered. I want to use data from real-time GPS tracking and a Raspberry Pi to orient the rocket back to where it came from so it does not get lost. Along with that, the rocket can collect data, such as altitude, temperature, orientation, acceleration, and video from the rocket.

---

## About Me

I am a 7th grader at BC High in Dorchester, MA. I enjoy math, physics, model rocketry, robotics, and amateur radio. I have done FLL (First Lego League) for 5 years, and this year I am going to Greece for the world championships. I competed in the American Rocketry Challenge this year. I have my Technician license for amateur radio. I also won 3rd place for the ABMF Past Is Prologue essay contest for my age group. Outside these, I do competitive swimming for my local swim team, and I am learning how to play tennis.

---

## How It Works

When the rocket goes up, once it reaches apogee (the peak of its flight), the wings swing out from the sides of the rocket and the model starts to glide down. The Raspberry Pi will use real-time data to calculate how to orient itself back towards the launch site. Servos will move the rudder and elevator surfaces to control the descent. During all of this, the sensors on the rocket will collect additional data, such as altitude, acceleration, and video from the point of view of the rocket glider.

The swing wing design of the wings is inspired by the GLSDB (Ground Launch Small Diameter Bomb), which uses wing sweepback for roll and yaw stability. The rocket will likely use D, E, and F engines.

---

## Electronics

The computer that will control everything is the Raspberry Pi Zero 2W, and the sensors will all be from the BerryGPS-IMU v4 from Ozzmaker. I will have 2 micro servos connected to the computer to move the control surfaces on the glider. The camera I will use is the Raspberry Pi Camera Module 3, connecting to the Raspberry Pi using the dedicated FPC cable that connects to the Raspberry Pi Zero. The Raspberry Pi and sensors will be powered by a 1200 mAh battery with the PowerBoost 1000C from Adafruit. The servos will be connected to a separate rail using the Pololu U3V70F5 step-up voltage regulator.

### Wiring Diagram

![Wiring Diagram](https://github.com/jediquinlan/GPS-guided-rocket-glider/blob/main/wiring.png?raw=true)

---

## Materials

- Paper tube (rocket body)
- 1/8" balsa wood (wings and fins)
- 1/16" plywood (structural components)

---

## Cost Breakdown

| Component | Cost |
|---|---|
| Raspberry Pi Zero 2W with headers | $20.70 |
| BerryGPS-IMU v4 | $74.00 |
| Raspberry Pi Camera Module 3 | $38.50 |
| Raspberry Pi Zero FPC camera cable | $3.95 |
| 1200 mAh LiPo battery | $9.95 |
| PowerBoost 1000C | $19.95 |
| Pololu U3V70F5 | $22.95 |
| 2x Hitec HS-55 Micro Servo | $33.98 |
| **TOTAL** | **$223.98** |

---

![Glider Diagram](https://github.com/jediquinlan/GPS-guided-rocket-glider/blob/main/glider_darkened.jpg)
