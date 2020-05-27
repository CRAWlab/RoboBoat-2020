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

# April 7, 2020

## Meeting Agenda
1. Open discussion of progress, suggest new ideas
2. Coordinate based on what everyone has worked on where efforts should be diverted and who should collaborate more closely.

## Discussion
### RTabMap
Received clarification about, because the ZED outputs so many different types, RTabMap should expect to see over the topics when remapping. Discussed difference between rectified and unrectified images.

`rosbag` files from the 2019 competition will be available for download soon to build a map using this package. The current `rosbag` files on OwnCloud are only about 15 seconds of data. Nathan and Ben, and maybe Dallas, will work on this more closely on this when Nathan is more available after Thursday.

### Image Labels
Although it was included in the last report comments, clarification over the current state of the image labeling was provided by Dr. Vaughan. We're still in the process of getting things fixed there, but we have a training set of 2500 images that was used for an agent to label the next 7000 or so. We will need to correct these labels on the 7000 once the issues are resolved.

### Report Expectations and Recap
Ben reiterated that team members could and should comment on the reports that are available on Github. ***The reports are meant to be an open discussion***.

### Enclosure Upgrade Discussion
Joseph talked about how Bradley, Thomas, and himself are having regular meetings, and have decided to pursue development of the air-cooled enclosure using hydrophobic mesh membranes. Recent developments included a few part selections and high-level logistics of what is and is not necessary of the cooling. Any airflow is a plus.

Joseph is also working on a SolidWorks Flow simulation to study the airflow and temperature gradients. Ben encouraged him to reach out to Jacob Deshotels, Jacob Randall, and Lane Elder, who have also done work with CFD for the waterjet propulsion system design.

### Tutorial Work, Tentative Collaboration
* Ben and Nathan (and maybe Dallas): RTabMap
* Ben and Gerald: Control System Discussion once the navigation stack is mostly configured
* Joseph, Andrew, Bradley, Thomas: Enclosure Development
* Dallas, Gerald, Nathan: ROS Wiki Tutorials -- Publisher/Subscriber, Navigation (Husky, Heron, Turtlebot)

# April 14, 2020
## Meeting Cancelled - Lack of noteworthy advances

# April 21, 2020
## Meeting Cancelled - Spring Break

# April 28, 2020

## Discussion
1. Competition changes, interest for 2021 competition (forwarding the funds)
2. Availability of team members given finals' week and semester wrap-up obligations
3. PDF of 2019 report will be available soon -- will need to change a lot around new discussion
4. Since stay-at-home order extended through May 15, team members will be gridlocked on physical collaboration ability until then
5. Will look at prior years' team videos for how to prepare that part of the digital submissions
6. No word on the need for a technical design presentation, yet
7. Website design will likely be done using https://pages.github.com, https://help.github.com/en/github/working-with-github-pages
8. RoboNation Website opens submissions for digital media competition components this week. May have closing deadline.
9. Need to have more discussion and collaboration to get these tasks done.

# May 5, 2020
## Deadlines
Talked about the new deadlines RoboNation has outlined via email:

### REQUIRED
1. Team Information: DUE May 22, 2020
2. Advisor Information: DUE May 22, 2020
3. Website: DUE June 7, 2020
* Gerald and Ben, perhaps more, will be collaborating on this the morning of May 6, 2020. We will host Zoom calls throughout this process. Will be working using Github website tools.

4. Technical Design Report: DUE June 21, 2020
* Aiming for a first draft out to Dr. Vaughan sometime during first week of June.

5. Team Video: DUE June 28, 2020
* Brief introduction of team members. Does not focus on the boat design.

### OPTIONAL
1. Create a Task: DUE July 5, 2020
2. Systems Engineering Paper: DUE July 12, 2020
3. Resume/CV: Rolling Deadline

### Miscellaneous
1. There will be an online awards ceremony held (tentatively) during the week of July 26, 2020.
2. There will be a video call this week hosted by RoboNation to go over submission requirements. To be held on either May 7 or 8.
3. Registration refund or forward to 2021 competition needs to be filled out by May 11, 2020.

# May 12, 2020
1. The guidelines for the digital submissions can be found at: https://robonation.org/app/uploads/sites/3/2019/10/Team-Submissions_RB20-Online.pdf. The major changes from last week's understanding is that the video is supposed serve as a substitute for the in-person competition presentation as well.

2. Gerald, Ben, and Nathan will work on the controller development using the Clearpath Heron as a base. Dallas also, possibly.

> ***BA*** Today, I confirmed that my Heron installation works and launches, and I outlined the launch process and what nodes get launched by the Heron. I plan on working on this more tomorrow (5/13) while my simulations are running. I know the last time you came into town, you mentioned that you were working on a RoboBoat Gazebo simulation. Do you have the models ready to create a custom robot?

3. Bradley, Joseph, and Thomas will continue working on development of the enclosure. The goal is to have some initial CAD modeling done for next week so, if needed, their efforts can be devoted to other aspects of the system and helping to write.

4. I'm waiting on the following media content for the website:
	a. 2019 team member pictures and emails
	b. Email for Andrew
	c. Pictures of Andrew, Nathan, Dallas

## Due Dates
### Required
1. Team Information - DUE May 22, 2020
2. Advisor Information - DUE May 22, 2020
3. Website - DUE June 7, 2020
4. Technical Design Report - DUE June 21, 2020
5. Video - DUE June 28, 2020

### OPTIONAL SUBMISSIONS
6. Create a Task - DUE July 5, 2020
7. Systems Engineering Paper - DUE July 12, 2020
8. Resume / Curriculum Vitae (CV) - Rolling Deadline

# May 19, 2020
1. Gave a verbal explanation of the two branches I created yesterday and what they're used for.
	a. Created a `current_software` branch with all of the packages currently on the RoboBoat because there seems to be a disparity between `master` and the boards.

	b. Created a `dev` branch with the Gazebo packages I'm working on.

I explained how cloning the repository should pull all branches, but we will want to keep them separate, and that any commits made to those branches will not show up in Slack channels until the branches are merged to `master`.

2. Discussed the Gazebo simulation, current state, what's left to add.
	a. I'm going to try using either the previous `roboboat_description` package that wasn't cloning as a new starting point or that ROS package you linked for SolidWorks parts today.

	b. Velocity curve fitting for baseline quadratic drag fits -- equation form should match WAM-V because of hull structure.

	c. Alternatives to `mpc.pytorch` -- will probably try `ACADO` first because I think I was able to get a linear model working. I'm converned about requiring `|v|` in one of the linear drag terms, though, as it does not like to optimize absolute values.

3. Discussed image classifier, how to implement. Gerald and Thomas thought that just running a node that uses Tensorflow, or whatever was used to train the classifier, is how it's done, but I have very little knowledge about this. Dallas could not make this meeting, so I'll discuss with him later today. I did mention to him last week that I have little knowledge about this subject.

4. Enclosure Discussion
	a. Joseph, Bradley, and Thomas would like some sort of bound on how much "future-proofing" needs to go in the enclosure. How much of the extra space do they need to/want to utilize to add a second Jetson, etc? Although there are only two so far, how different is the footprint of a TX1 vs a TX2 vs TX(i) from generation to generation?

	b. Can enclosure footprint cover up the holes in the hull bridge that are currently used to pass motor control wires? They would still be used, but probably passed from the bottom of the enclosure if so, rather than drilling new holes.

	c. They are really concerned with getting estimates for what their final temperature of the box should be, but since their objective is just "reduce" and not "reduce by X", I've informed them to spec out a fan that fits and does not consume too much power, and calculate "if ambient temp is `x`, boards are emitting `y` through free convection, with volume flow rate `vdot`, what is `qdot` out of the box?" rather than hit a target temp.

	d. Mentioned using a snorkel as cover for inlet and exit holes. I don't think this is a great idea for airflow reasons, but it might not be a huge difference.

	e. Is the max temp reached at 2019 competition a good benchmark for operating temps to base calculations off of?

	f. Will be designed as if we were adding another TX2 to the box.
5. Website
	a. Trying to encourage team members of taking pictures doing _whatever_ they're working on to add to website. Planning for next meeting (5/26) to have everyone's webcams on for at least part of it for someone to take a picture of everyone communicating.

	b. Not sure why my picture isn't showing up, but will take a new one to replace. Image file might be corrupted or something.

	c. Going to resize everyone's images to match uniform square. Is there an easier way to do this than just adjusting height/width tags?

	d. Waiting on pictures from Andrew, Nathan.

	e. Did you ever get in contact with the old team? None have responded to my message on Slack.

6. Still shooting for a report draft first week of June. The enclosure team is using this as a target date for their results.

# May 26, 2020

Andrew and Nathan were not able to attend the meeting due to work. 

1. Discussed where I (Ben) am at with the Gazebo simulation
	a. Need to correct the position of the pose sensors, but they should be uniquely identified in Gazebo

	b. Need to combine the image data with laser scans in `RTabMap`

	c. Need to spawn buoys to test the image classification running through `darknet_ros`

	d. Need to take classified images and output towards local path planner using way points. Not sure what algorithm yet. Asked Gerald, and he described some of the different ones, but did not explicitly recommend any particular one.

	e. Need to create a controller using `ACADO` that receives info about the local trajectory from the path planner and outputs a `Twist()` msg on `/cmd_vel` or `/cmd_drive`.

	f. Need to map the `Twist()` msg to the motors.

I expressed that I don't fully know what I'm doing, and would appreciate help in setting it up. I'll post in the Roboboat channel when I'm working on it again, but devoting most of my efforts towards my thesis.

2. Discussed the fan options found by the enclosure team.
	a. There was a little confusion in either where the fan should go or describing the same thing to each other. I tried to explain that the fan needs to go inside of the enclosure, behind a mesh/screen that keeps water out.

	b. Most of these fans operate around 120-150 CFM, which seems a little excesive. They've mentioned that you advised them to look at 123mm fans. I've advised them to steer away from 24 VDC fans, as it's probably more trouble than it's worth to cool everything using that. There is a word doc with the fans and a description with a location of where they found them on McMaster-Carr, but no actual URLs. It's currently in the Slack DM between Joseph, Thomas, Bradley, and myself, and hopefully stored on someone's computer besides my own.

	c. In this list of descriptions, all amperages are listed. I told them, but have not confirmed, that the power calculations you think were done by the 2019 team were likely in their technical report. The max amperage on the listed fans is  about 0.8-0.9A, so I don't think it will be an issue. I, again, reiterated that we're not trying to spec a fan because we need to cool the enclosure `x` degrees, but we're trying to pick a fan that fits, is power-friendly, and blows some air.

	d. Since the meeting, I know you've discussed with Joseph about a possibly pre-fabricated enclosure with built-in fans, or something to that effect. He found something and showed me on Zoom, but I don't have a link to it. I assume you two are in frequent communication. This enclosure he found does weigh about 15 lbs more than the existing, though.

3. Mentioned the report and website deadlines. Received radio silence back. I might try and tackle resizing those images today with that tag/property you mentioned last week. I should have some downtime waiting for sims to finish up before I have enough to write about conclusively.