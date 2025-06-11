# mtrn4010---project-1-solved
**TO GET THIS SOLUTION VISIT:** [MTRN4010 – Project 1 Solved](https://mantutor.com/product/mtrn4010-project-1-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;72648&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MTRN4010 – Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
<strong>MTRN4010 – Project #1 (Parts C-F) </strong>

<h1>Basic Data Fusion</h1>
&nbsp;

In this task we commence using (and processing) data from multiple sensors, simultaneously. We do it in a simple way: deterministically. These are preliminary steps, which are useful for solving the localization problem through stochastic Sensor Data Fusion, which will be applied in subsequent project 2.

This task involves processing multiple sensing capabilities: LIDAR, wheel encoder and gyroscope (yaw rate, from IMU).

All the modules which are implemented in this task will be used for solving part of a subsequent project. Properly solving this task does not only give you a good mark in this task, but also facilitates the solution of that subsequent project.

One of the purposes of this task is for understanding and implementing localization by applying “deadreckoning”. The second purpose is getting used to using different coordinate frames and for implementing a Data Association process. All of them are necessary for the subsequent project.

&nbsp;

&nbsp;

<strong>Part C</strong>.

&nbsp;

Implement a function for estimating the attitude of the platform, based on the measurements of the IMU’s gyroscopes. You may assume that the platform is always operating in a 2D context; consequently, you can assume that the pitch and roll are always =0; which allows processing the integration by simply integrating the yaw angular rate 𝜔<sub>𝑧</sub>. The measurements, to be processed in this task, are provided in the file “IMU_dataC.mat”.

&nbsp;

Verification of results: For verifying the performance of your implementation, you will use the data provided in the file “IMU_dataC.mat”; you will integrate the yaw gyroscope’s measurements, and plot the estimated attitude, for the full duration of the test (whose duration was about 250 seconds). You will compare it (by simply inspection) with a solution provided by the lecturer, and, also, by verifying that the initial and final conditions “make sense”, by visually inspecting the laser scanner images (which were taken from the vehicle, during the same test). The laser scanner data is provided in the file “Laser__2C.mat”.

&nbsp;

Relevance of this part: 20% (of the full mark of this project)

<strong>&nbsp;</strong>

<strong>&nbsp;</strong>

<strong>Part D. </strong>

&nbsp;

You are required to implement a “dead-reckoning” process, based on the kinematic model of the platform and the measurements provided by sensors (speed encoder and gyroscope). The kinematic model was explained in the document “[AAS_2020]_KinematicModels.pdf”. The way for implementing it is explained in that document, as well.

The inputs of the process model are the angular rate 𝜔<sub>𝑧</sub> and the speed encoder measurements. The necessary data is contained in the Matlab data files “IMU_dataC.mat” and “speed_dataC.mat”. These files do also include useful comments (in addition to the necessary data and sample times) for explaining the data format.

&nbsp;

Validation: You will compare the estimated path (by simply inspection) with a solution provided by the lecturer. Additional validation of these results will be done in Part E.

&nbsp;

Relevance of this part: 20%

&nbsp;

<strong>Part E </strong>

&nbsp;

At each time, when a laser scanner measurement is available, you will perform the following processing:

&nbsp;

<ul>
<li>Obtain an estimate of the position and orientation of the platform at that time (provided by part D).</li>
<li>Perform feature extraction, for detecting the OOIs (as implemented in Project1)</li>
<li>Express the currently detected OOIs’ positions in a global coordinate frame (using the results obtained in (1) and (2))</li>
</ul>
&nbsp;

We assume as “global coordinate frame” the one aligned with the platform at time t<sub>0</sub>. I.e. we say that the platform’s position and heading at time t<sub>0</sub> are (x=0 m, y=0 m) and (heading=90 degrees) respectively (based on the coordinate frame convention, shown in figure 1).

For proper processing, you must consider the position of the laser scanner (on the platform), as it is shown in figure 1. The displacement, <strong><em>d</em></strong>, is 46 cm (approximately), longitudinally.

&nbsp;

<strong>Figure 1 </strong>

&nbsp;

Expected result: When the currently detected OOIs are shown in the global coordinate frame, they would appear near the original OOIs, detected at the initial time. The discrepancy will be increasing as the platform travels, due to the cumulated error in the platform’s pose estimates (an error which usually grows with the time).

&nbsp;

Validation/Visualization of results: For showing the performance of this process, your program will plot (dynamically, as you have done in previous tasks), the OOIs detected at the initial time and the OOIs currently being detected. Both sets of OOIs will be shown in the global coordinate frame. Use different colors and/or symbols for each set of OOIs.

&nbsp;

Relevance of this part: 20%

&nbsp;

<strong>&nbsp;</strong>

<strong>Part F</strong>

&nbsp;

Implement a Data Association process.

Based on the previous parts of this task; implement a Data Association (DA) process. The DA concept is discussed in class (week 4).

The DA process would be able to identify (and keep identifying) the OOIs that are detected at each scan. The operation of the module is expected to be the following one:

<ul>
<li>At scan #0, the ranges are processed for inferring the OOIs which are present in the image. Those are given identities, i.e. a unique number for each of them, and their positions registered.</li>
<li>Each subsequent scan is also processed for extracting the OOIs occurring in it. The DA process will infer the identity of each currently detected OOI, based on the positions of the OOIs obtained in the first scan and on the estimated global positions of the currently detected OOIs. A tolerance of 40 cm will be considered for the matching process.</li>
</ul>
For visualizing the performance of the approach, you will use Part C, adding text nearby each currently detected OOI, for indicating its inferred ID.

&nbsp;

Expected performance: In this case, considering that the localization process is simply based on the dead reckoning of the platform, we expect you to achieve a successful DA during, at least, the first 10 meters of the trip.

Relevance of this part: 20%
