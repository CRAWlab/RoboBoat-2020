# RoboBoat 2020 Meeting Minutes
## Team Members:
### Faculty Advisor -- Dr. Joshua Vaughan -- joshua.vaughan@louisiana.edu
1. Captain: Benjamin Armentor -- benjamin.armentor1@louisiana.edu
2. Alternate Captain: Joseph Stephens -- joseph.stevens1@louisiana.edu
3. Gerald Eaglin -- gerald.eaglin1@louisiana.edu
4. Dallas Mitchell -- dallas.mitchell1@louisiana.edu
5. Nathan Madsen -- nathan.madsen1@louisiana.edu
6. Thomas Poche -- thomas.poche1@louisiana.edu
7. Andrew Durand -- andrew.durand1@louisiana.edu
8. Bradley Este -- bradley.este1@louisiana.edu

## Competition Rules: https://robonationforum.vbulletin.net/forum/roboboat/-2020-roboboat/2542-rules-tasks

## Project Boards
### Media: https://github.com/CRAWlab/RoboBoat-2020/projects/1
### System Development: https://github.com/CRAWlab/roboboat/projects/1

# March 24, 2020
## Meeting Agenda
1. Determine what tasks of the competition will be attempted
2. Discuss who wants to work on what subsystem(s)
3. Introduce proposed high-level system design
4. Familiarize team with available resources
5. Show team members how to install and work with ROS

## Discussion
The team decided that the following tasks will be attempted:
* Navigation Channel
* Obstacle Channel
* Obstacle Field
* Speed Gate
* Return to Dock
* Docking (without hydrophone)

The following tasks will ***NOT*** be attempted:
* Object Delivery (likely through UAV)
* Docking with Hydrophone

Also discussed the option of purchasing a secondary ZED stereo camera to mount to the stern of the RoboBoat to facilitate holonomic motion, ugrading networking to Ubiquiti equipment from the WAM-V.
* What is the footprint of this equipment compared to the TP-Link equipment?

Internal reporting procedures and expectations were briefly discussed. The next team report is due on **April 1, 2020**. Team members have also been made aware of the project boards and repositories available through CRAWLAB's GitHub page. The repositories can be found with relative ease from the project board links above.

Primary objective is to get everyone familiarized with working in ROS during the stay-at-home order. Fridays from 1-3 have been dedicated as team work days, as everyone marked this as available time slots. It is expected that team members will also work individually outside of this.

Team members have been encouraged to reach out to others for help if they encounter issues with ROS installation or usage.

Team members have been instructed to work on ROS tutorials and commit their progress in their *personal* code folders -- **NOT** the RoboBoat repositories.

## Sub-group assignments:

These are subject to change as tasks are completed or as unexpected difficulties arise, and certain tasks require more workload.

### Enclosure Upgrade Research, Installation
* Joseph
* Andrew
* Thomas
* Bradley

> ***BA*** Must be *at least* IP67 rated, relatively lightweight, and bigger than current enclosure (22x12x8 inches).

### Control System Development
* Ben
* Gerald
* Joseph
* Nathan

> ***BA*** Starting with navigation stack to get appropriate outputs of `cmd_vel` messages to a lower-level controller. Differences between Model Predictive Control and Model Reference Control were discussed, but this decision will ultimately come after the navigation stack is working properly.

### Computer Vision System Training
* Dallas
* Thomas

> ***BA*** Awaiting images uploaded by Dr. Vaughan to be linked for ***everyone*** to start labeling. Will be located at: `labelbox.com`. Documentation available at: `https://labelbox.com/docs`.

