+++
title = '2024 10 22 Ninth Fall Meeting'
date = 2024-10-23T11:37:23-04:00
draft = false
summary = 'asteroids direction/progress, meeting times'
tags = ['meeting', 'playdate', 'project', 'schedule']
+++
***
# Overview
- Attendance
- Asteroids Project
	- Direction
	- Recent PRs
- Semester Meeting Times
- Next Week
***
# Attendance
Officers:

- Abu Shettima
- Lavender Wilson
- Matthew Williams
- Paul Shriner

Members:

- Chibuikem Asuzu
- Kevin Kauffman
- Maddox Miller
- Michael Paterno
# Asteroids Project
## Direction
Since the project has been taking up a lot of club time, we plan on having a small segment at the beginning of each meeting (~30 minutes at most) discussing any new developments.
## Recent PRs
There have been 2 recent pull requests on the project:
- One implementing shooting from the ship (Kevin's PR)
- One refactoring and reorganizing the file (Lavender's PR)
### Lavender's PR
- Implements a new state machine 
	- A global variable holding a string determinse what state function to call
- Reorganized each function into globals and each state
### Kevin's PR
- Allows the player ship to shoot a projectile
- Only one projectile may be on the screen at once
	- Code is in place for more to be added if necessary
- Projectile stops at the screen egde (does not wrap around)
- Currently uses button callback functions
	- May update to Playdate's `InputHandler`s in the future
# Semester Meeting Day/Time
We discussed changing the meeting day to Friday (which would allow us to have earlier meetings), but decided against it because the current day and time works for most of us.

We'll be discussing next semester's meeting day/time once people get their schedules sorted out (and sometimes classes change even after that, so the exact day and time may still change). 
# Next Week
We'll be doing a meeting talking about Linux! We'll discuss things like:
- Differences from Windows
- Terminal/CLI tool familiarity
- Differences between distributions and desktop environments

Several of those involved in the club use Linux on a daily basis and will be providing their thoughts and experiences with it, so don't be afraid to ask any questions!

The meeting will take place the same day and time as usual (Tuesday, 5-6p). 