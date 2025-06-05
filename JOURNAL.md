---
title: "Zetaboard"
author: "Akshat Khurana"
description: "An ergonomic, wireless and productivity optimised 65% keyboard!"
created_at: "2024-06-04"
---

## 4th of June: Ideation.
I'm honestly so hyped for this project and today was all about spending some time consolidating this hype into actual features to implement onto a keyboard. After watching a bunch of long Youtube videos on the topic, notably Christian Selig's ["I Built My Dream Keyboard from Absolute Scratch"](https://www.youtube.com/watch?v=7UXsD7nSfDY&t=1179s) and Modern Hobbyist's underrated ["I Built My DREAM Keyboard from SCRATCH (and it's modular)"](https://www.youtube.com/watch?v=KwFWBdfZKnI), I had a good idea of things I wanted in my keyboard, what I really did not want and also some pretty clever tools I can use in the process.

So in terms of layout and size, I've decided to stick to a QWERTY layout (boring, I know, but I use my laptop keyboard a ton and don't want to learn the ins and outs of a completely custom layout) on a 65%-ish keyboard. In the Zetaboard, I want to do away with some of the keys I've basically never used, or intend to in the future. And, to increase productivity, I'm going to be integrating a Pomodoro timer into the keyboard. TL;DR, these are my main features:

- Hot swappable MX switches
- 65% + a few knobs (get rid of never-used keys)
- Inbuilt pomodoro timer (special key and layer for it)
- RGB, or some form of backlighting
- Wireless
- Vertically tilted slightly, so that each key is slightly above the one below (ergonomics)

I got into Keyboard Layout Editor, to do up a quick visual of what I have in mind. It'll look something like this.

![alt text](images/annotated_layout.jpg)

I've added a special Zeta key which will used to trigger a layer for the Pomodoro timer and other keyboard related actions.

I've gotta start looking for some parts now...

**Total time spent:** 3h

## 5th of June: Part Sourcing.
This morning, I showed my design to a friend, and he made some suggestions which I've added into my KLE design;

![alt text](images/updated_layout.jpg)

I've basically just shifted some keys around to make sure the main letter keys are centered and the other keys go around, while still leaving space for the rotary encoders and Pomodoro timer.

In total, I've got 61 keys, and the Capslock, Enter, Shift and Space keys will need stabilisers - not too sure how to implement in the PCB, but we'll cross that bridge when we get there...

I'm also not too sure about the MCU I'm going to use - from what I've heard, Nice!Nano is pretty good, but there's one small problem; it only has 21 GPIO pins, and I need a good amount more, for my 7-segment display and rotary encoders (I'll be having 4 of those in total).

In total I need 19 GPIO for my switches, 2 GPIO for my display and another 4 for the buttons on the rotary encoders (I'll be wiring)