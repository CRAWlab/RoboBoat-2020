<h1 style="text-align:center;">Ragin' Cajuns RoboBoat</h1>

*****
Welcome to the [University of Louisiana at Lafayette](https://louisiana.edu)'s entry into the 
[2020 RoboBoat competition](https://roboboat.org). This is Ragin' Cajuns' second design submission to RoboBoat.

<div style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
    <a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48428302362/in/photostream/" title="More Pool Testing - 3"><img src="https://live.staticflickr.com/65535/48428302362_ecf03cd3fd_5k.jpg" alt="More Pool Testing - 3"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 0%">
    <a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48135383553/" title="2019 International RoboBoat Competition - 125"><img src="https://live.staticflickr.com/65535/48135383553_690469da5a_5k.jpg" alt="2019 International RoboBoat Competition - 125"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div><br>

Our team is coached by [Dr. Joshua Vaughan](https://userweb.ucs.louisiana.edu/~jev9637/people.html), an Associate Professor at the University of Louisiana at Lafayette. This year's Ragin' Cajun RoboBoat Team members are all [Mech. Engineering](https://mche.louisiana.edu/) students from Dr. Vaughan's research group, [C.R.A.W.LAB](https://userweb.ucs.louisiana.edu/~jev9637/index.html).

The 2019 Ragin' Cajuns RoboBoat team, who fabricated the hull and laid the groundwork for us to build on, were all graduating seniors in Mechanical Engineering. While all of the students are in the same discipline, the 2020 Ragin' Cajuns have students at many different points in the program. This has allowed for many great mentoring opportunities within the team.

*****

<!-- Coach -->
<h2 style="text-align:center;">Ragin' Cajuns RoboBoat Team</h2>
<h3 style="text-align:center;">Coach</h3>
<p align="center">
	<img width="20%" src="Figures/MemberPhotos/JoshuaVaughan.jpg"/><br>
	<b style="text-align:center;">Dr. Joshua Vaughan</b><br>
	<i style="text-align:center;">joshua.vaughan@louisiana.edu</i><br>
</p>

*****

<!-- Captains -->
<h3 style="text-align:center;">2020 Team Members</h3>

<div style="float:left;text-align:center">

<p style="float:left;text-align:center; width: 20%; margin-right: 20%; margin-left: 20%">
	<strong style="text-align:center;">Captain</strong><br>
	<img width="100%" src="Figures/MemberPhotos/BenjaminArmentor.JPG"/><br>
	<b style="text-align:center;">Benjamin Armentor</b>
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 20%; margin-left: 0%">
	<strong style="text-align:center;">Vice Captain</strong><br>
	<img width="100%" src="Figures/MemberPhotos/JosephStevens.jpg"/><br>
	<b style="text-align:center;">Joseph Stevens</b>
</p>

</div>

<!-- Additional Members -->
<!-- Row 1 -->
<br>
<div style="float:left;text-align:center">
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 10%">
	<img width="100%" src="Figures/MemberPhotos/GeraldEaglin.jpg"/><br>
	<b style="text-align:center;">Gerald Eaglin</b>
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 0%">
	<img width="100%" src="Figures/MemberPhotos/NathanMadsen.jpg"/><br>
	<b style="text-align:center;">Nathan Madsen</b>
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 0%">
	<img width="100%" src="Figures/MemberPhotos/DallasMitchell.JPG"/><br>
	<b style="text-align:center;">Dallas Mitchell</b>
</p>
</div>

<!-- Row 2 -->
<br>
<div style="float:left;text-align:center">

<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 10%">
	<img width="100%" src="Figures/MemberPhotos/ThomasPoche.jpg"/><br>
	<b style="text-align:center;">Thomas Poché</b>
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 0%">
	<img width="100%" src="Figures/MemberPhotos/AndrewDurand.jpg"/><br>
	<b style="text-align:center;">Andrew Durand</b>
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 0%">
	<img width="100%" src="Figures/MemberPhotos/BradleyEste.jpg"/><br>
	<b style="text-align:center;">Bradley Este</b>
</p>
</div>

<!-- Row 3 -->
<br>
<p style="float:left;text-align:center; width: 20%; margin-right: 40%; margin-left: 40%">
	<img width="100%" src="Figures/placeholder.PNG"/><br>
	<b style="text-align:center;">Kyle Leleux</b>
</p>

<h2 style="text-align:center;">Design Changes</h2>
The main focus of this year's entry was a code cleanup and new control strategy. Unfortunately, the 2020 RoboBoat in-person competition has been cancelled, so this design will not get to physically compete. This, along with sanctions placed by our state and local governments and university, has stifled some of the manufacturing improvements to the design, but the details are flushed out in the documentation.

The 2020 Ragin' Cajuns RoboBoat still uses [ROS](http://wiki.ros.org/) as the computer network's communication platform. We have improved the computer vision system by adding an additional [ZED Stereo Camera](https://www.stereolabs.com/zed/). We have adjusted our SLAM from [gmapping](http://wiki.ros.org/gmapping) to [RTab-Map](http://wiki.ros.org/rtabmap). Lastly, the control code has been overhauled to use Model Predictive Control using the [ACADO Toolkit](https://acado.github.io/). This control method enables mathematically optimal control by minimizing a cost function that we define.

On the hardware side, we wanted to expand our enclosure to allow for more computing power and add a cooling system. The enclosure has been redesigned to raise it off of the hull's bridge to allow for an array of fins to absorb the heat through conduction from the enclosure and expel it through natural convection while at rest, but forced convection when the vessel has surge motion. The manufacturing was not completed, but the design is complete. A huge thanks go out to Hammond Manufacturing and AWC for their generous donations.

<h2 style="text-align:center;">Development</h2>

<!-- Row 1 -->
<div style="float:left;text-align:center">
<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img  src="Figures/YOLO.jpg" alt="Testing the image classifier"/>
</p>

<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 0%">
	<img width="290" height="218" src="Figures/RQT.png" alt="ROS RQT graph of node network"/>
</p>

</div>

<!-- Row 2 -->
<div style="float:left;text-align:center">
<br>
<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img src="Figures/Floating_heron.png" alt="Things didn't always go as planned"/>
</p>

<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 0%">
	<img src="Figures/Troubleshooting.png" alt="Team conference call fixing Gerald's sinking RoboBoat"/>
</p>

</div>

<!-- Row 3 -->
<br>
<div style="float:left;text-align:center">
<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img src="Figures/HeatSink.PNG" alt="CAD drawing to model heat sink for new enclosure"/>
</p>

<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 0%">
	<img src="Figures/OldEnclosure.PNG" alt="Old enclosure design"/>
</p>

</div>

<!-- Row 4 -->
<br>
<div style="float:left;text-align:center">
<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img src="Figures/NewZED.PNG" alt="Adding the new ZED stereo camera to the CAD assembly"/>
</p>

<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 0%">
	<img src="Figures/NewLIDAR.PNG" alt="Adding new Hokoyu LiDAR to the CAD assembly"/>
</p>

</div>

<!-- Row 5 -->
<div style="float:left;text-align:center">
<br>
<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img src="Figures/NewEnclosureMounting.PNG" alt="Adjusting the rail system to support the raised enclosure"/>
</p>

<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 0%">
	<img src="Figures/NewEnclosureMountedWithLid.PNG" alt="New enclosure on rail system, equipped with heat sinks"/>
</p>
</div>

<br>

<h2 style="text-align:center;">Documentation</h2>
* Technical Design Report (to be linked soon)
* Team Video (to be linked soon)

*****

<h1 style="text-align:center;">2019 Ragin' Cajuns</h1>
<p align="center">
	<strong style="text-align:center;">Captain</strong><br>
	<img width="20%" src="Figures/placeholder.PNG"/><br>
	<b style="text-align:center;">Christian Gary</b><br>
	<!-- <i style="text-align:center;">TBD@something.com</i><br> -->
</p>

<!-- Row 1 -->
<br>
<div style="float:left;text-align:center">
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 10%">
	<img width="100%" src="Figures/placeholder.PNG"/><br>
	<b style="text-align:center;">Luke Matt</b><br>
	<!-- <i style="text-align:center;">TBD@something.com</i><br> -->
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 0%">
	<img width="100%" src="Figures/placeholder.PNG"/><br>
	<b style="text-align:center;">Kaleb Gautreaux</b><br>
	<!-- <i style="text-align:center;">TBD@something.com</i><br> -->
</p>
<p style="float:left;text-align:center; width: 20%; margin-right: 10%; margin-left: 0%">
	<img width="100%" src="Figures/placeholder.PNG"/><br>
	<b style="text-align:center;">Grant Bellard</b><br>
	<!-- <i style="text-align:center;">TBD@something.com</i><br> -->
</p>
</div>

***** 

<h2 style="text-align:center;">Highlights</h2>
<!-- Row 1 -->
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 2.5%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/32882767317" title="RoboBoat Pseudo-FBD Sketch II"><img src="https://live.staticflickr.com/65535/32882767317_03ccd6f38b_q.jpg" width="150" height="150" alt="RoboBoat Free-Body Diagram"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 0%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48135381943/in/album-72157707215763765/" title="Not a bad first year"><img src="https://live.staticflickr.com/65535/48135381943_32588c5e1c_3k.jpg" width="150" height="150" alt="Not a bad first year - Winners of Manufacturing Award"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 0%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/47594323382/in/album-72157707215763765/" title="RoboBoat Electronics"><img src="https://live.staticflickr.com/65535/47594323382_fbe1c21973_3k.jpg" width="150" height="150" alt="RoboBoat Electronics"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>

<!-- Row 2 -->
<br>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 2.5%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48135464462/" title="2019 International RoboBoat Competition - 21"><img src="https://live.staticflickr.com/65535/48135464462_603cebba84_3k.jpg" width="150" height="150" alt="2019 International RoboBoat Competition - 21"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 0%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/46744293214/in/album-72157707215763765/" title="RoboBoat hull fabrication"><img src="https://live.staticflickr.com/7884/46744293214_a94d7a7539_3k.jpg" width="150" height="150" alt="RoboBoat Hull Fabrication"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 0%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48135405193/in/photostream/" title="2019 International RoboBoat Competition - 8"><img src="https://live.staticflickr.com/65535/48135405193_ed3bd1bae9_3k.jpg" width="150" height="150" alt="2019 International RoboBoat Competition - 8"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>

<!-- Row 3 -->
<br>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 2.5%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48097796362/in/album-72157707215763765/" title="Sunny Thursday morning at RoboBoat"><img src="https://live.staticflickr.com/65535/48097796362_1b4d12c5ac_3k.jpg" width="150" height="150" alt="Sunny Thursday Morning at RoboBoat"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 0%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48135395133/in/album-72157707215763765/" title="2019 International RoboBoat Competition - 57"><img src="https://live.staticflickr.com/65535/48135395133_38288a4c17_3k.jpg" width="150" height="150" alt="2019 International RoboBoat Competition - 57"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>
<div style="float:left;text-align:center; width: 30%; margin-right: 2.5%; margin-left: 0%">
	<a data-flickr-embed="true" href="https://www.flickr.com/photos/crawlab/48135356281/in/album-72157707215763765/" title="2019 International RoboBoat Competition - 87"><img src="https://live.staticflickr.com/65535/48135356281_76ecb7d580_3k.jpg" width="150" height="150" alt="2019 International RoboBoat Competition - 87"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
</div>

<h2 style="text-align:center;">Documentation</h2>
* [Technical Design Report](ULL_RB19_TDR.pdf)
* [Team Video](https://www.youtube.com/watch?v=DXaP6OPKAoY&feature=youtu.be)

*****

<h2 style="text-align:center;">Our Sponsors</h2>
<p style="text-align:center">
This project would not be possible without the donations from our sponsors.

<br>

Thank you all for your generosity and support.
</p>

<!-- Row 1 -->
<br>
<div style="float:left;text-align:center">
<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img width="100%" src="Figures/Sponsors/hammondmfg.PNG" alt="Hammond Manufacturing"/><br>
</p>

<!-- [Website](https://www.hammfg.com) -->

<p style="float:left;text-align:center; width: 45%; margin-right: 3.33%; margin-left: 3.33%">
	<img width="100%" src="Figures/Sponsors/logo_awc.jpg" alt="AWC Industrial"/><br>
</p>

<!-- [Website](https://www.awc-inc.com/) -->

</div>

<h2 style="text-align:left;">Contact Us</h2>
* Email: benarmentor@gmail.com
* Phone: 1-(337)-967-6860