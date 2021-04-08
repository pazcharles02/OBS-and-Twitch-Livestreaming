---
layout: default
title: Capturing Display with Source
nav_order: 3
---

## Sources Overview

Now that you have created a scene, you can now build the look of your stream by layering sources on it.
Think of your scene as the stage for a theatrical play. The sources you add are the moving set pieces that your audience will see.

Please direct your attention to the Sources module and press the '+' button: 

![Source Empty](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_Empty.png?raw=true)

You should see a menu similar to the one below:
*For your convenience, we have highlighted the most commonly used sources for livestreaming*

![Source Add Menu](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_add_menu.png?raw=true)
- [Display Capture](#capturing-your-entire-screen): Get your entire screen
- [Game Capture](#capturing-a-game): Capture a fullscreen application / game
- [Window Capture](#capturing-a-window): Capture a specific window (e.g. A web browser)
- [Video Capture Device](#capturing-camera-feed-or-external-device): Get feed from a connected webcam, camera, or other external capture device

*When using Game Capture or Window Capture, the application you wish to capture must already be running for OBS to detect it.*

## Capturing Your Entire Screen

Select Display Capture. The properties window should appear.

![Display Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_Display_Properties.png?raw=true)
1. Select your monitor from the drop-down menu
2. If you do not want the audience to see your cursor, uncheck the 'Capture Cursor' box
3. Press 'OK'

## Capturing a Game

![Game Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/GameCaptureProperties.png?raw=true)

1. We recommend using the mode 'Capture Specific Window', as this gives you the most control over which application OBS detects and captures.
2. Select your app/game from the drop-down 'window' menu
3. Press 'OK'

If you cannot find your currently running application in the drop-down menu, try searching for it using a Window Capture source instead.

## Capturing a Window

![Game Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_Window_Cap_Properties.png?raw=true)

1. Select your window from the drop-down menu 
2. Verify that the window you want to capture has appeared in the preview
3. Press 'OK'



Should you need to change these capture settings at any time, right click the source, view properties, and select a different program to capture from the drop-down menu.

## Capturing Camera Feed or External Device
*If your stream does not require your audience to see your computer screen (e.g. Use of camera to record a fitness sessions), skip to capturing camera.*
Ensure your recording device is connected to your computer
Create a new 'Video Capture Device' source
Select your device from the drop down menu and press OK.
