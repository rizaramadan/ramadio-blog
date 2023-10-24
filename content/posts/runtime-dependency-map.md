+++
title = 'Runtime Dependency Map'
date = 2023-10-23T15:02:32+07:00
draft = false
+++
Lets just say that in order to sustain, we need to improve. And to improve, basically we need to move. Speaking about movement, in real life, what is the tool that is commonly and widely used to move from one place to another? It's a map.
Map is a model to provide us information about the current landscape we are in. It helps us articulate clearly where we are in, where we want to go, and how the movement will be from here to there.
That’s the “map” part, and what is the deal about “runtime dependency”? As we all should know, our system generates values when it runs, and it's paramount that we keep it stable. Keep it mind it's not as easy as it sounds because too many things can go wrong. And more often than not, problems come from uncontrolled dependencies. 
Hence, Runtime Dependency Map is a map for us to know where we are currently with our services and dependencies, it will tremendously help us to figure out where we need to improve and where we want to be ideally.

Runtime dependencies map is inspired by Wardley Mapping
https://learnwardleymapping.com

# What
A map is basically a diagram where every place means something. Think of a cartesian diagram, it can be considered a map, whereas a mindmap can’t.
In Runtime Dependency Map:
X-Axis, Up and down means movement on system's dependencies, upper sections means more direct dependencies, lower section means more deep dependencies
Y-Axis, Left and right means movement on stability
