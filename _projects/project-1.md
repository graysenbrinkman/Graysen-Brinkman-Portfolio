---
layout: research
title: "AIRHOUND Research Project"
category: "Research & Clubs"
section: "research"
date_range: "Aug 2025 – Apr 2026"
image: /assets/images/airhound-thumb.jpg
description: "A drone system designed to track and follow other flying objects."
skills: [PX4, SITL, HITL, ROS2, LaTeX]
overview: "AIRHOUND (Autonomous Intelligent Rotorcraft for Hostile Unidentified Navigation and Detection) is an 8-person research project at Embry-Riddle Aeronautical University's Engineering Physics Propulsion Lab. The project's goal is to detect and track airborne objects in real time, with applications in aerospace, military, and naval domains. The system runs on an NVIDIA Jetson Orin using the ROS2 Humble uXRCE-DDS framework."
contribution: "On this project, I helped integrate the PX4 converter node into our drone framework, which let the flight controller and onboard Jetson Orin compute communicate reliably over ROS2's uXRCE-DDS middleware. I also configured our Software-in-the-Loop (SITL) and Hardware-in-the-Loop (HITL) testing pipelines, which is a critical step for catching issues in simulation before they ever reached a live flight test. Alongside this, I co-authored Section 2 (Methods) for our team's paper, published in an undergraduate research journal."
status: "Published"
paper_link: "https://commons.erau.edu/cgi/viewcontent.cgi?article=1176&context=beyond"
gallery:
  - src: /assets/images/gazebo-test.png
    caption: "Conducting Software-in-the-Loop on the drone using Gazebo"
  - src: /assets/images/airhound-poster.jpeg
    caption: "Presenting our research poster at an Embry-Riddle Research Symposium"
learned: "AIRHOUND taught me how tightly software and hardware have to work together in a real-time system, where small timing issues between the flight controller and onboard compute can cascade into real problems. Running SITL and HITL tests reinforced the value of catching failures in simulation rather than in the field. It also sharpened my technical writing skills."
---