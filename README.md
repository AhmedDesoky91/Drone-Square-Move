# **Drone Square Move**
---

**In this project, I have worked on the development of high level motion commands of quadcopter drone using python under the simulator of Udacity's Flying Cars and Autonomous Flight Nanodegree.**

## Project Description and Architecture:
---
### Project General Description
In this project, I have worked on writing a pyhton script which allows a drone in a simulator to fly in a backyard.
The aim of the project is provide the commands that is similarly communicated from a flight computer and an autopilot. 

### More Details
In the world of autonomous flight and drones development, most of the time you will be writing programs that run on the flight computer. And these are the highest level programs that for example might decide where the vehicle should go next, and guide the vehicle along a sequence of way points by properly setting the vehicle’s target position which is communicated to the autopilot.
The autopilot in turn communicates back crucial information like GPS measurements and IMU data.
All of this communication happens using some sort of a connection. In a real drone, this connection might be a USB connection. In the simulator, this is a subclass of a connection class.

The following diagram visualized what is stated above more simply :

![img1](https://i.imgur.com/CaK6TpW.png)


### Project Architecture and States
- The project is based on event-driven programming Paradigm
   - Event-driven programming is a programming paradigm in which the flow of execution is determined by external events rather than a pre-defined sequence of steps.
   - The way of linear sequential programming will not work properly with controlling our drone.
Because mainly, we set some set of commands, this will block the code from doing any other things.And we want to react dynamically to our environment and our mission.

- Project States
   -  To accomplish the mission of our project, we need to through different states
   -  To move from a state to another, there should be an event that triggers the transition.
   -  The following diagram viualizes the different states and transitions in our project :

![img2](https://i.imgur.com/Fgmx1xA.png)


## Environment:
---
* Ubuntu 18.04 LTS
* Udacity FCND Simulator
   * https://github.com/udacity/FCND-Simulator-Releases/releases
* UdaciDrone
   * https://udacity.github.io/udacidrone/docs/drone-api.html
* Miniconda
* Python 3

For setting up the environmernment and how to use the simulator, check the [FCND Backyard Project Repo](https://github.com/udacity/FCND-Backyard-Flyer).

