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

# March 31, 2020

## Meeting Agenda
1. Communicate issues with ROS install
2. Update team on details of RoboNation Conference Call - March 29, 2020
3. Recover expectations of Team Report - Due 4/1/2020
4. Open conversation about enclosure upgrade, led by Joseph
5. Tutorial Work

## Discussion

### ROS Installation Issues
* Will add a VirtualBox disk image to Owncloud for others, so everyone is working from same platform. This should resolve any installation issues, though some may have trouble downloading it.

### RoboNation Conference Call
Go/No Go Final Decision on competition will be made on April 24
* Navy Volunteers
* Gathering limits imposed by local/state gov't of FL
* Facility usage
* Cancellation policy will be adjusted for this -- can opt for either refund of registration or, if it's an accounts issue to get refund, then a forward to 2021 competition

RoboNation is currently not considering throttling the number of people allowed per team to meet gathering requirements, if they're raised from 10, but still imposed

Robonation is currently not considering postponing rather than cancelling

To keep a sense of community, RoboNation will start hosting both technical and non-technical webinars
* First on Thursday, April 2, 2020 (non-technical): Blue Origins: Company Opportunities
* Will try to be announced 4-5 days in advance over Band App, but depends on vendors' response times
* Example of technical would be Mathworks showing an ad-hoc tutorial
* All will be recorded and uploaded EXCEPT Q&A with vendor approval
* Webinars will be hosted every 2 weeks

***DO NOT share links to webinars outside of team members***

Invitation Letters go out week of April 6, 2020, mostly for people/teams who need Travel Visas

### Team Report
Each team member/sub-team (CV, Enclosure, Control, etc.) will write up progress individually following style of `CRAWLAB/Internal Reporting`

Report writeups are expected by 5pm on the due date

Reports serve as template for technical buildup of system for report due to RoboNation as part of competition


### Enclosure Upgrade Discussion
Discussed Joseph's, Bradley's, and Thomas' current idea(s)
* Water-cooled system with downward-facing outspout mounted near CoG to prevent additional moments
* Simplifications for calculations, such as assuming water temperature is uniform
* Heat sink with water-reservoir to absorb the heat from the mounting plate

Reintroduced idea of hydrophobic/water-wicking membrane to get airflow rather than developing a complex, water-cooled system

Next enclosure team meeting is evening of 3/31/2020

### Tutorial Work
I (Ben) will be working on configuring the navigation stack using the `rosbag` files from the past competition as tuning tools
* Next will be downloading `ZED` and interfacing that output with `rtabmap`. I expect to do this Friday afternoon.

Recommended Dallas get started with basic ROS tutorials on publishing/subscribing and then working up towards working with `ZED` since he will be CV lead.

Joseph will be continuing to work through the ROS book and then with turtlebot tutorials.

