Video Compression

`Philipp` `(website)`[http://www.philkr.net/]

---

## Why Video is hard?
1. image capture enough information (at least some "intersting" part is missing)
2. most camera are image camera, not video (not anymore)
3. too big (compression, their work)
4. labeling (only true for real image)

## Motivation
- Information theory: original 2MB-> decompress to 500MB. You scatter the information to sparser video

## Work
- Too large --> compression(his work)
    + learn a recognition on top of current compression codec
    + learn to compress video without recognition (compared to MPEG, etc)
    + NEXT?? combine them together
- Label --> video game. self supervised learning
    + simulation. video game
    + the hard only happens in real data
- Are they 

## QA
- Katerina: Computation Issue
    + specialized chips(for now)
- Kris: what if AE are too big. You just distribute the storage offline.   
- A1: What is the question(task) you are trying to solve in video?
    + faster? slower? causality? 
    + Answer: Architecture side is general. It's not tailored to specific task. task and architecture(I3D) are two things. What is the task that you really NEED video.
-  Katerina: Video has even less information. coz lots of movement is only due to camera!!
