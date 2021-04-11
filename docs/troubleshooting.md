---
layout: default
title: Troubleshooting
nav_order: 7
---

## Troubleshooting

## Game Capture Issues

**I cannot find my game in the Game Capture Source properties.**

Run OBS or your game in administrator mode. Sometimes games are not recognized by OBS for capture unless in administrator mode.

**My game is being detected, but the preview just shows a black screen.**

If your game is running in fullscreen mode, this means that you will not see the game in the OBS preview while it is minimized. You can verify that your game is being detected by the following:

- Move OBS to a second monitor to see if the preview changes when you reopen the game
- Start a recording, then watch the video that is saved locally on your computer (Usually in your main hard drive 'Videos' folder').
- Begin streaming and ask viewers to check that your game is being captured correctly.

If the above fails, try running your game in either windowed or fullscreen borderless mode, and use a Window Capture source instead. Some games do not respond well to OBS game capture in fullscreen mode.

## Computer Performance Issues

Remember that in addition to running your program/game, your computer now has to work additionally hard to stream it. 

1. Try lowering the output resolution of your stream
Go to Settings -> Video -> Output (Scaled) Resolution. Choose a lower resolution and test your stream again until you are satisfied with the performance. Note that you should keep your Base (Canvas) Resolution the same.

If you are choosing to downscale your resolution, the different downscale filters (Bilinear, Area, Bicubic, and Lanczos) will also have some impact on your performance.
Bilinear is the best choice for maximizing performance. Lanczos is the best choice for maximizing image quality.
Test your stream to determine with which filter satisfies your performance needs.

2. Try lowering the output framerate of your stream
Go to Settings -> Video -> Common FPS Values. If you are streaming at 60 FPS, choosing a lower value will increase performance.

3. Remove/Modify Sources
Any source that exists on your scene takes up computer resources. Take care to remove unnecessary sources that you are not currently using.

If you are using a webcam/camera that isn't being displayed fullscreen on your stream, try lowering its capture resolution. To maximize performance, your webcam feed in the corner of the screen should not need be encoded in any greater than 720p.


## Stream Quality Issues

Lower your bitrate.

OBS Studio 24 introduced a new feature called Dynamic Bitrate. This feature detects when your internet connection is limited, and will automatically reduce your bitrate to compensate rather than dropping frames. Once any congestion disappears, it will automatically raise your bitrate back to its original value.

To enable Dynamic Bitrate, first ensure you are using OBS Studio 24 or higher by looking at your version number in the title bar of the program. Then, go to Settings > Advanced > Network and check the box next to the option that says "Dynamically change bitrate to manage congestion".
