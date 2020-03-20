---
title: "Internet Beats" # Title of your project
date: 2020-03-20T13:34:12-04:00
weight: 0 # Order in which to show this project on the home page
external_link: "" # Optional external link instead of modal
draft: true
---

This is [my first open source software](https://pub.dartlang.org/packages/internet_beats) package. I'd like to build a [Flutter](https://flutter.io/) mobile app (Android and iOS) that displays the time in Internet Beats. [Internet Beats](https://www.timeanddate.com/time/internettime.html) were invented about twenty years ago by Swatch, and offer a location-independent, zone-less method of telling time. It's sort of like UTC, but it breaks the day into 1,000 "beats," rather than hours, minutes, seconds, etc. Unsurprisingly, there's no library that manages time in Internet Beats, so I decided to write one as a first step.

This is a bit of a hack, in that I haven't created anything that keeps time in a fundamnetally different way. It merely takes a local or UTC time and algorithmically converts it. It depends on the system its run on to have the time set correctly. For most mobile devices, this probably isn't a stretch. And the way it's written, an app using the library could call a time service before using the library to be certain the time's right.
