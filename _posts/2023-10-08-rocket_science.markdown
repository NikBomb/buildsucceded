---
layout: post
title:  "It's rocket science"
date:   2123-10-08 08:00:00 +0000
categories: [simulations, javascript]
---

## Introduction

Last month we have all awed to the Chandrayaan-3 mission, where mankind has for the first time landed near the Moon South pole.
Inspired by the landing images, I decided to re-approach the topic of propulsion since my time at uni. In this post I will derive the rocket equation, trying to get familiar with variable mass systems. Then I will integrate the equation in time under as set of not so stringent hyothesis, and to convince myself of the correctness of the integration, I will present a simulation, in the form of an interactive game, in Javascript, that can run in your browser. Finally I will present a sub-optimal strategy to beat the game, using the suicidial burn manoeuvre.

## The rocket equation 
<img src="/assets/images/rocket/ConservationMomentum.png" width="500" style="display: block; margin: 0 auto">

I start from a rocket, or whatever orbiting object in space with some thrusters, in a vacuum under the influence of gravity. 
Acceleration equation

The interesting thing about lunar modules is that they can contain as much as 60% of their total mass as propellant for the descent stage like the Apollo 11 (https://nssdc.gsfc.nasa.gov/nmc/spacecraft/display.action?id=1969-059C). This data is important because it invalidates Newton's second law, that only applies to mass invariant systems. To better understand the physics at play we will examine how the Lander using its engines, contrasts lunar gravity.

The engine is capable of accelerating a mass of propellant, so we can analyze the system lander and propellant mass, before and after this acceleration, using the principle of conservation of motion to this system.

Image here.

And equation. 

Using a first principle we have been able to derive the equation of motion for the lander. In particular, the effect of propulsion is equivalent when using a little mass expelled at high velocity or a big amount of mass expelled at a slower velocity. In this analysis we can simply include a gravity term as a constant working in opposition to the propulsion term.

Equations of motion 

For simplicity, we will keep our motion in 1d (up or down). Another simplification is that we will imagine that the mass will vary over time with a constant prescribed rate. Under these assumptions, our aim is to obtain the velocity and position at every time of the descent.
Using the power of math the velocity and position as function of time can be derived as:


Now we are able to fully describe the descent phase of the Lander in 1d in case of a single constant burn rate or a sequence of constant burn rates.

Simulation



