---
layout: page
title: HeatSchedule — Energy-aware heating for EPFL rooms
description: A LauzHack 2022 build — a Python framework that schedules room heating from real occupancy data, cutting energy use without compromising comfort.
importance: 2
category: hackathon
img: assets/img/proj2.jpg
github: https://github.com/Thomas-debug-creator/LauzHack
---

Built in **24 hours at [LauzHack 2022](https://lauzhack.com/)** with *Martin Zwifl* and *Thomas Rimbot*: a framework for scheduling room heating in EPFL buildings based on actual occupancy, designed to reduce energy use while preserving comfort.

## The problem

University buildings heat empty rooms by default. EPFL has detailed room-reservation data per building, but no system uses it to drive HVAC schedules — heating runs on fixed timetables that ignore when rooms are actually booked. The wasted energy compounds across hundreds of rooms over a winter.

## Approach

A Python framework with three parts:

- **Occupancy signal** — pulls room reservation schedules directly from EPFL's booking system. Rooms with no reservations in a given time window are flagged as candidates for heating cutbacks.
- **Heating curve parameterisation** — each room has a configurable thermal model (warm-up time, set-point, decay rate) so the scheduler can pre-heat a room before its next reservation without over-shooting.
- **Simulation framework** — runs the schedule against a parameterised building model and reports projected energy savings vs. the baseline fixed schedule.

The whole thing is object-oriented so individual rooms, buildings, and heating policies can be swapped without rewriting the core scheduler.

## Result & scope

A working 24-hour proof of concept that ingests EPFL reservation data and outputs heating schedules, plus a simulation environment to compare strategies. The natural next step is wiring the scheduler to a real HVAC controller — the abstraction layer is there, but live integration was out of scope for the hackathon.

<i class="fa-brands fa-github"></i> **Code:** [github.com/Thomas-debug-creator/LauzHack](https://github.com/Thomas-debug-creator/LauzHack)
&nbsp; · &nbsp;
<i class="fa-solid fa-link"></i> **Devpost:** [devpost.com/software/heatschedule](https://devpost.com/software/heatschedule)
