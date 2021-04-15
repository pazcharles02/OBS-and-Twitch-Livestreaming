---
layout: default
title: Capturing Display with Source
nav_order: 3
---

## Sources Introduction

Now that you have created a scene, you can now build the look of your stream by layering sources on it.

Think of your scene as the stage for a theatrical play. The sources you add are the moving set pieces that your audience will see.

## Add a Source

1\. Press the '+' button under the Sources module: 

![Source Empty](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_Empty.png?raw=true)

You should see a menu similar to this:

![Source Add Menu](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_add_menu.png?raw=true)

*The most commonly used sources are highlighted in red.*

2\. Select the type of source that best suits your needs:
- [Display Capture](#capture-your-entire-screen): Capture your entire screen
- [Game Capture](#capture-a-game): Capture a fullscreen application / game
- [Window Capture](#capture-a-window): Capture a specific window (e.g. A web browser)
- [Video Capture Device](#capture-camera-feed-or-external-device): Get feed from a connected webcam, camera, or other external capture device

*When using Game Capture or Window Capture, the application you wish to capture must already be running for OBS to detect it.*

After selecting a source type, OBS should prompt you with this screen:

![Source Add Menu](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_create.png?raw=true)

3\. Select 'Create New' and enter a name for your source.

4\. Press 'OK'

## Capture Your Entire Screen

When you create a Display Capture source, the properties window should appear like this:

![Display Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_Display_Properties.png?raw=true)
1. Select your monitor from the drop-down menu
2. If you do not want the audience to see your cursor, uncheck the 'Capture Cursor' box
3. Press 'OK'

## Capture a Game

When you create a Game Capture source, the properties window should appear like this:

![Game Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/GameCaptureProperties.png?raw=true)

1. Select 'Capture Specific Window' in the 'Mode' drop-down menu (This gives you the most control over which application OBS detects and captures)
2. Select your app/game from the drop-down 'Window' menu
3. Press 'OK'

If you cannot find your currently running application in the drop-down menu, try searching for it using a Window Capture source instead.

## Capture a Window

When you create a Window Capture source, the properties window should appear like this:

![Game Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_Window_Cap_Properties.png?raw=true)

1. Select your window from the drop-down menu 
2. Verify that the window you want to capture has appeared in the preview
3. Press 'OK'


Should you need to change these capture settings at any time, right click the source, view properties, and select a different program to capture from the drop-down menu.

## Capture Camera Feed or External Device

When you create a Video Capture Device source, the properties window should appear like this:

![Camera Capture Properties](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_cam_properties.png?raw=true)

1. Find your connected device in the 'Device' drop-down menu (The preview window should show your live camera/device feed)
2. Select 'Custom' Resolution/FPS Type
3. Select the highest resolution value for your device (Usually the one at the top of the list)
4. Select 'Highest FPS'
5. Select 'Full' Color Range
6. Press 'OK'

## Basic Source Manipulation

Now that you have created a couple of sources, we will summarize how to use OBS's interface to structure and edit your sources.

**Note: The order of the sources in the Sources list directly reflect the layout of sources in your scene.**

In the following screenshot, Video Capture Device sits above Zoom Window Capture in the Sources list, thus allowing the webcam feed to appear in front of the zoom window. 

![Source Manipulation Legend](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/assets/images/Source_manu_legend.png?raw=true)

1. This preview shows how your stream will look to your audience. Modify the position of a source by clicking it in the preview, then drag it into place or resize as desired.
2. This 'eye' button indicates if a source is visible. Toggle it on/off to change the visibility of a source in your scene.
3. This 'padlock' button indicates if a source is modifiable. It is useful if you have many sources on screen and you do not want to make changes to them. Toggle it on/off to lock/unlock editing for a source.
4. Use this '+' to add additional sources to your scene.
5. After selecting a source, press this '-' button to delete it from your scene.
6. After selecting a source, press this cogwheel to view the properties for the source.
7. After selecting a source, use these arrow keys to move the source up or down a layer. Alternatively, you can reorder your sources by dragging and dropping with your mouse.

## Conclusion

Congratulations! You should now have some sources set up. 
You are very close to being ready to start your first stream. 
Now head over to [Capturing Audio](https://pazcharles02.github.io/OBS-and-Twitch-Livestreaming/docs/capturing-audio/) to learn how to capture various audio feeds for your stream.
