---
layout: default
title: Troubleshooting
nav_order: 7
---

## Troubleshooting

## Game Capture Issues

Question: "I cannot find my game in the Game Capture Source properties."

Answer: Run OBS or your game in administrator mode. Sometimes games are not recognized by OBS for capture unless in administrator mode.


Question "My game is being detected, but the preview just shows a black screen."

Answer: If your game is running in fullscreen mode, this means that you will not see the game in the OBS preview while it is minimized. You can verify that your game is being detected by the following:

- Move OBS to a second monitor to see if the preview changes when you reopen the game
- Start a recording, then watch the video that is saved locally on your computer (Usually in your main hard drive 'Videos' folder').
- Begin streaming and ask viewers to check that your game is being captured correctly.

If the above fails, try running your game in either windowed or fullscreen borderless mode, and use a Window Capture source instead. Some games do not respond well to OBS game capture in fullscreen mode.

## Computer Performance Issues

Remember that in addition to running your program/game, your computer now has to work additionally hard to stream it. 

**1. Try lowering the output resolution of your stream**

Go to Settings -> Video -> Output (Scaled) Resolution. Choose a lower resolution and test your stream again until you are satisfied with the performance. Note that you should keep your Base (Canvas) Resolution the same.

![Trouble Resolution](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/trouble-resolution.png?raw=true)

If you are choosing to downscale your resolution, the different downscale filters (Bilinear, Area, Bicubic, and Lanczos) will also have some impact on your performance.
Bilinear is the best choice for maximizing performance. Lanczos is the best choice for maximizing image quality.
Test your stream to determine with which filter satisfies your performance needs.

**2. Try lowering the output framerate of your stream**

Go to Settings -> Video -> Common FPS Values. If you are streaming at 60 FPS, choosing a lower value will increase performance.

**3. Remove/Modify Sources**

Any source that exists on your scene takes up computer resources. Take care to remove unnecessary sources that you are not currently using.

If you are using a webcam/camera that isn't being displayed fullscreen on your stream, try lowering its capture resolution. To maximize performance, your webcam feed in the corner of the screen should not need be encoded in any greater than 720p.


## Stream Quality Issues

If you are experiencing framedrops while streaming, this is an indication of a network issue. 
Try lowering your video bitrate:
Go to Settings -> Output -> Video Bitrate

![Trouble change bitrate](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/trouble-change-br.png?raw=true)

Your internet speed determines your bitrate limit. Run the [Ookla Speed Test](https://www.speedtest.net) and record your upload speed (measured in Mbps).

Here are some setups that you can use based on your upload speed:
---

1080p 60 fps (Full HD, high framerate)

Recommended upload speed: 6.5 to 8+ Mbps

Resolution: 1920 x 1080

Bitrate: 4500 to 6000 kbps

Framerate: 60 fps

---

720p 60 fps (HD, high framerate)

Recommended upload speed: 5.5 to 7 Mbps

Resolution: 1280 x 720

Bitrate: 3500 to 5000 kbps

Framerate: 60 fps

---

1080p 30 fps (Full HD, standard framerate)

Recommended upload: 5.5 to 7+ Mbps

Resolution: 1920 x 1080

Bitrate: 3500 to 5000 kbps

Framerate: 30 fps

---

720p 30fps (HD, standard framerate)

Recommended upload speed: 4.5 to 6 Mbps

Resolution: 1280 x 720

Bitrate: 2500 to 4000 kbps

Framerate: 30 fps

---

480p 60 fps (SD, high framerate)

Recommended upload speed: 3.5 to 5 Mbps

Resolution: 640 x 480

Bitrate: 1500 to 2500 kbps

Framerate: 60 fps



OBS Studio version 24+ includes a new setting called Dynamic Bitrate. This feature detects when your internet connection is unstable, and will dynamically adjust your bitrate for you while streaming. Using this setting should reduce instances of dropped frames. 

Go to Settings -> Advanced -> Network 

Check the box: 'Dynamically change bitrate to manage congestion'

![Trouble audio bitrate](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/trouble-autobitrate.png?raw=true)
