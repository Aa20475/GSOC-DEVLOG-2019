**Project Name:**  Motion Matching Implementation In Godot

**My Name:** Aditya Abhiram (_aka **DestinyGamer**_)

**Mentors:** Juan Linietsky([@reduz](https://github.com/reduz)) and Thomas Herzog([@karroffel](https://github.com/karroffel))

**GIT Repo:** [godot-motion-matching](https://github.com/Aa20475/godot/tree/godot-motion-matching)

# Motion Matching Implementation in Godot!

First of all, I want to thank the Godot project and my mentors, Juan Linietsky and Thomas Herzog, for giving me a chance to work on this project.

I'm so excited to share my experience while working with this project! This project changed my perspective towards open source.

## Motivation:

Godot, is an open-source game engine, was built with a  _never-ending wish of adding new features to it_.

Motion Matching is one of the latest features in Game Animation which is quite revolutionary. Usually, setting up a basic animation system needs a lot of work and time. Even after that, we barely manage to make a perfect one. Motion matching, on the other hand, is a method where the computer chooses the best pose for each frame by itself from a huge database of mocap data using some Algorithm.

> Choose the best pose for each frame and jump to it!

#### This wonderful feature needs to be included in Godot!

## What was the plan?
 - Starting by implementing simple Pose and Trajectory matching using Brute force approach.
 - Building on it by adding KDTree for optimization.
 - Experimenting with it as much as possible!

## How it went!
This project has three parts :

 -   Cost function
 -   The future trajectory prediction model
 -   KD-Trees for KNN search (Optimisation)
 

 #### *Community Bonding Period*
I started getting familiar with Godot API and trying to implement simple projects in it. I also got familiar with my mentor and other developers. 

#### *Coding Period #1 (May 27,2019 - June 24,2019 )*
We started by collecting datasets for testing while @reduz worked on the UI of the Editor. By mid-June, reduz made a basic structure where I need to plugin my functions in. And by the time of First Evaluation, I had a barebones KDTree and KNNSearch up and running!

#### *First Evaluation Period ( June 24,2019 - June 28,2019)*
I tried implementing a basic future trajectory prediction function.

#### *Coding Period #2 (June 28,2019 - July 22,2019)*
I started building a Simple Pose and Trajectory Matching System which uses a brute force approach and Added some UI improvements. Started working on some small crashes and minor details.

#### *Second Evaluation Period (July 22,2019 - July 26,2019)*
Fixed some bugs and errors in the system.

#### *Coding Period #3 (July 26,2019 - August 19,2019)*
Started working on exposing needed parameters to the users. 
Bugs persisted but worked my best to fix stuff. Tried to replace brute force approach with KDTrees. It worked but considerably heavy. ***(Needed Optimization)***  Started working on fixing parameter issues *(It is not choosing while playing the Scene because of these errors)*.

#### *Final Work submission Period (August 19,2019 - August 26,2019)*
Still stuck up with the parameter passing issues.