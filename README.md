![banner](https://github.com/antoinesylvia/antoinesylvia/blob/main/banner.jpg)
![](https://komarev.com/ghpvc/?username=antoinesylvia&color=grey) Hanging out at the National Videogame Museum in Frisco, Texas.

------------------------------
# My Github Projects

Just a spot where I put projects I've worked on or currently working on. Code and documentation. 

-------------------------
* [Texas Heat Raceway](https://github.com/antoinesylvia/Texas_Heat_Raceway) - This project [currently under development over the next few months], implements an automated 6 lane racetrack system for diecast vehicles 1/64 scale, featuring real-time race management, result tracking, audio-visual feedback and more. The track operates outdoors under a covered roof in Dallas, Texas. My power users for testing are my 3 year old son and 6 year old daughter. 
![Texas Heat Raceway in Action](https://github.com/antoinesylvia/Texas_Heat_Raceway/raw/54fa975025f74245992fad0b8fe581977904259c/zPics/20240816_225830.jpg)
The system is comprised of:
- Start Gate: Beginning of track, uses Lego motors via a Raspberry Pi Build HAT for automation.
- Checkpoint Gate: Bottom of the initial launch incline, wtih light sensors, powered via a Raspberry Pi.
- Finish Gate: End of the track, with light sensors, powered by a Tiny Lenovo ThinkCentre, but can be swapped out for a Pi.
- Central Server: Serves as the brain of the operation, handles the coordination and race event state between the start gate, checkpoint gate and finish gate.
- Audio Manager: Plays various sounds based on race state.
- Web Control Interface: Ran locally, main dash, race events and configuration options.
- Leveraging of the I2C as a backbone for each gate, extended with the STEMMA QT Ecosystem. Allows us to communicate between multiple devices/sensors/displays via a multiplexer, using just two wires: SDA (data line) and SCL (clock line). 
- Measurement of stats per car rolled out in 5 parts. We aim to measure and analyze the physical properties of HotWheels cars as they move along the track, from basic speed and energy calculations to advanced physics like force, energy efficiency, and momentum changes. This comprehensive analysis helps us understand the cars' performance, optimize track design, and improve overall race dynamics.
  - Part 1: Basic Measurements
    - Speed: Measure how fast the car moves.
    - Kinetic Energy: Calculate the energy the car possesses due to its motion.
    - Momentum: Determine the car’s momentum, the product of its mass and velocity.
    - Distance Traveled: Measure the total distance the car covers during the race.

  - Part 2: Advanced Measurements (requires checkpoint data)
    - Acceleration: Calculate the rate of change in the car’s speed over time.
    - Gravitational Acceleration: Measure the effect of gravity as the car moves down the incline.

  - Part 3: Force and Energy (requires acceleration/gravitational data)
    - Force: Measure the force acting on the car due to acceleration.
    - Potential Energy: Calculate the stored energy based on the height of the track.
    - Work Done: Calculate the work performed as the car moves over a distance.
    - Power: Measure the rate at which work is done by the car.
    - G-Force: Calculate the force relative to gravity that the car experiences.

  - Part 4: Advanced Physics
    - Rolling Resistance: Calculate the energy lost due to rolling resistance.
    - Energy Loss: Estimate the total energy loss due to friction and resistance.
    - Coefficient of Restitution: Measure how much kinetic energy is conserved during a collision.
    - Heat Generation: Calculate the heat generated due to friction.
    - Vibration Dynamics: Analyze how vibrations impact the car’s stability.
    - Torque: Measure the rotational forces acting on the car’s wheels.
    - Impulse and Jerk: Measure the change in momentum and the smoothness of acceleration.
    - Terminal Velocity: Determine if the car reaches maximum speed.

  - Part 5: Final Efficiency Calculations
    - Mechanical Efficiency: Calculate how efficiently the car converts input energy into motion.
    - Energy Transfer Efficiency: Measure the efficiency of converting potential energy into kinetic energy.
    - Coefficient of Friction: Determine the friction between the car’s wheels and the track.
    - Energy Conversion Efficiency: Calculate the efficiency of converting energy from the start to the finish.
    - Impulse and Momentum Change: Calculate how the car’s momentum changes as it transitions on the track.
   
![Texas Heat Raceway Setup](https://github.com/antoinesylvia/Texas_Heat_Raceway/raw/f776e179d2016afa6b6089f81d7a35401d6e4603/zPics/20240816_225454.jpg)
---------------------
* [Adblock Load Balancer](https://github.com/antoinesylvia/adblock_load_balancer) - Tool to forward raw DNS requests to the PiHole/Adguard with the least load (2+ required). Built for home LAN usage, my agents run on gen 1 Raspberry Pi units which I wanted to make use of as a summer project for 2023. Components here include: Agents script (pushes server usage stats where PiHole/Adguard is installed), Metrics script (collects real-time server usage information from agents) and Load Balancer main script (uses data pulled from metrics to make a decision):
![load_balancer](https://raw.githubusercontent.com/antoinesylvia/adblock_load_balancer/main/z_pics/load_balancer.PNG) 
---------------------
* [GPT-4 with Vision Analyzer](https://github.com/antoinesylvia/dfw_metroplex_vision_gpt) - CLI utility built with Python which leverages OpenAI's GPT-4 with Vision to get information for your images. I wanted to play around with the new Vision feature that came out of the OpenAI developer day:
![Vision](https://github.com/antoinesylvia/dfw_metroplex_vision_gpt/blob/bc356d0626113e7fdf89c08d73170c675c8ada94/zzDemo/CLI.png)
---------------------
* [Lego Train Powered Up Automation](https://github.com/antoinesylvia/dfw_metroplex_poweredup_train) - Leverages Pybricks firmware, Lego Distance and Color Sensor, and Bluetooth! I have 2 Projects, 1 leverages hub-to-hub communication to enable 2 locomotives to work together utilizing a beta firmware. A 3rd project coming this summer (2023) will utilize a Raspberry Pi, Pi Build Hat for Lego and Remote. Demo links are included from my TikTok. This is a project built to support my kids Hotwheels track. 

  ![Lego Train Powered Up Automation - Project 1](https://github.com/antoinesylvia/dfw_metroplex_poweredup_train/blob/8380397289f0077545aec01b9a945f6d8fc9f5ff/zz_train_demo/project1.gif)
  ![Lego Train Powered Up Automation - Outdoor Test](https://github.com/antoinesylvia/dfw_metroplex_poweredup_train/blob/8380397289f0077545aec01b9a945f6d8fc9f5ff/zz_train_demo/outdoor_test.gif)
  ![Lego Train Powered Up Automation - Project 2](https://github.com/antoinesylvia/dfw_metroplex_poweredup_train/blob/8380397289f0077545aec01b9a945f6d8fc9f5ff/zz_train_demo/project2.gif)
---------------------
* [Kubernetes Cluster](https://github.com/antoinesylvia/Autoplex-Cluster) - My K3 cluster featuring many Raspberry Pis (bought used before the price explosion), Nvidia Nanos, and old x86/64 Thinkpads (collected over the years). The idea here is to scale out my self-hosted web apps (mostly from the [Awesome Self Hosted list](https://github.com/awesome-selfhosted/awesome-selfhosted) on GitHub), learn more about distributed computing, and implement GitOps (repo config holding the desired state). I share my computing resources with people I mentor and my friends who are security engineers.

  ![Kubernetes Cluster Hardware Info](https://github.com/antoinesylvia/Autoplex-Cluster/blob/a698782fab9cfef6df0b7fffd59080a50aa8da3a/hardware_info/lab.gif)
  ![Kubernetes Cluster Network](https://github.com/antoinesylvia/Autoplex-Cluster/blob/ab7a396ae3047457d9c3b55385e86922708b22ae/hardware_info/network.gif)
---------------------
* [Cloud Security Posture Management (CSPM)](https://github.com/antoinesylvia/pc-toolbox) - Originally forked from Palo Alto under MIT. Built scripts for a CSPM tool called Prisma Cloud. Added in the ability to do custom RBAC and user onboarding at scale (1000s of users and 1000s of projects) which wasn't native in 2020 and much more (compliance reports, alerts reports, backups, etc.). Forked but base project has about 2 scripts remaining out of the 50 I've added. Code structure is meant to be generic so users can plug in their own unique identifiers/parameters.

  ![CSPM](https://github.com/antoinesylvia/antoinesylvia/blob/c79f41d952ae252e547172428cb22b1b1f4f171e/z-cspm_.png)
  
* * * *

# Stats
[![My GitHub stats](https://github-readme-stats.vercel.app/api?username=antoinesylvia&theme=dark&show_icons=true)](https://github.com/anuraghazra/github-readme-stats)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=antoinesylvia&theme=dark&show_icons=true)](https://github.com/anuraghazra/github-readme-stats)

# About Me
![Boston](https://github.com/antoinesylvia/antoinesylvia/blob/f474daa30a7410869dbdd60be384bf89055ebd38/fenway.jpg)


-   :point_right: I am originally from the Boston Area ([city of Brockton](https://www.youtube.com/watch?v=icGphpZFYVw&t=1127s)), Celtics and Patriots fan! I miss summer in New England but not definitely not the winter.
-   :computer: What made me get into IT? When I was a kid, my Dad (Engineer) was always tinkering with electronics, building and coding things on the weekend (back in the DOS days). This sparked my curiosity, when I got to elementary school age, I began building and taking things apart to see how they worked, breaking my Mom's computer (hardware/software) a gazillion times, last one I can recall was an old Compaq Presario desktop that came with a Encarta 95 and Jet Moto CD. I eventually landed in a space where I became the defacto help desk computer guy for my family, friends and neighbors for a range of issues (to this day). Here's a quick link to the building of my homelab/office: https://imgur.com/a/iyYBpIc
-   :construction_worker: [Career Path](https://www.linkedin.com/in/antoinesylvia/): IBM [IT Architect -> Security Consultant] -> Sabre [Security Analyst -> Security Architect/Engineer] -> Activision Blizzard/Microsoft Gaming [Security Engineer] 
-   :monocle_face: Interested in helping others, mentoring and successfully prepping people for tech roles/interviews (IBM, Southwest, Citi, LinkedIn and more!). I also mentored youth over the course of several years in the Big Brother Big Sister program here in the Dallas area. I like helping people and paying it forward. 
-   :seedling: Currently learning more **Python**, **Ansible**, **Kubernetes**, **Terraform** and **ML/AI**.
-   :heart: Self-hosting software (helped me pivot into cybersecurity easier, attain certs quickly through lessons learned over the years in my homelab and importance of data privacy). My curated list: https://github.com/antoinesylvia/Autoplex-Cluster/tree/main/general_apps_info
-   :video_game: Retro gamer and collector (classic consoles/handhelds (70s to early 2000s)). 
-   :heart: My kids got me back into the world of diecast racing and Lego building.

-   :basketball: I am 6'8", but don't play basketball for my job (my most FAQ when I'm out) but I still get some time in when I take my kids to the playground! Still dunking.




![banner0](https://github.com/antoinesylvia/antoinesylvia/blob/main/dallas.PNG)
