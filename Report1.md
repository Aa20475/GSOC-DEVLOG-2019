**Project Name :**  Motion Matching Implementation In Godot

**My Name:** Aditya Abhiram (_aka DestinyGamer_)

**Mentors:** Juan Linietsky([@reduz](https://github.com/reduz)) and Thomas Herzog([@karroffel](https://github.com/karroffel))

**GIT 

## Introduction

Hey! This is Aditya Abhiram aka **DestinyGamer**. I am working on Implementation of Motion Matching in Godot.

Godot, being an open source game engine, was built with a *never-ending wish of adding new features to it*.

Motion Matching is one of the latest features in Game Animation which is quite revolutionary. Usually, setting up a basic animation system needs a lot of work and time. Even after that, we barely manage to make a perfect one. Motion matching, on the other hand is a method where the computer chooses the best pose for each frame by itself from a huge database of mocap data using some Algorithm.

>Choose the best pose for each frame and jump to it!

#### This wonderful feature needs to be included in Godot!


## Overview

This project has three parts :

* Cost function
* Future trajectory prediction model
* KD-Trees for KNN search (Optimisation)

We started off by collecting datasets for testing while @reduz worked on the UI of the Editor. I, along side data collection, tried out implementing KDTree and KNN search. The UI was ready by mid June and then I started adding and testing the KDTree and KNN search algorithms with it.

**`AnimationNodeMotionMatch` in `AnimationTree`:**

![AnimationNodeMotionMatch in AnimationTree](/Data/AnimationNodeMotionMatch.gif)


`AnimationNodeMotionMatchEditor` UI:

![AnimationNodeMotionMatchEditor](/Data/AnimationNodeMotionMatchEditor.png)


Just before the first evaluation , I successfully added KDtree and KNN search to the `AnimationNodeMotionMatch`.

During evaluation period, I tried making a simple future trajectory prediction models. 

After that, I started implementing **Pose and Trajectory Matching**(Calculating cost function using pose and root trajectory comparisons) without including KDTrees yet(*Just as a brute force attempt*). I'm still working on fixing the crashes in this matching.



## Next Steps:

* Getting Pose and Trajectory Matching running without any crashes.

* Adding Velocity Matching too so that the matching gets much natural.

* Taking past data into account during matching, so that we won't ignore weight-shifts and get a natural looking animation.

* Replacing the brute force approach with KNN search using KDTrees.

* Adding Sliders for parameters such as Pose vs Trajectory etc. 
