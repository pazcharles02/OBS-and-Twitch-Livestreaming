---
layout: default
title: Capturing Audio
nav_order: 4
---

## Capturing Audio

By default, OBS Studio should be configured to capture both your desktop audio and microphone input audio.
To test this, ensure that the volume bars in the audio mixer section properly display feedback based on audio activity.

1\. Play any audio through your computer's sound system. The 'Desktop Audio' volume bar should rise accordingly:

![Desktop Audio Bar](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/PC_AudioMixer.png?raw=true)

2\. Speak into your microphone. The 'Mic/Aux' volume bar should rise accordingly:

![Desktop Audio Bar](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/PC_AudioMixer_Mic.png?raw=true)

If you have a webcam or other connected device that can function as a microphone, it may appear in the Audio Mixer.
To prevent overlapping audio, we recommend that you mute such devices by clicking the speaker icon such that it looks like this:

![Desktop Audio Bar](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/PC_AudioMixer_webcam.png?raw=true)

To adjust the input volume of your audio devices, click and drag the sliders under each volume bar.

---

### Mac Setup for Capturing Audio Source (Skip Ahead to Step 9 for PC Users)

At this stage, you should have OBS downloaded and installed on your Mac.

**1.** Download and install iShowU Audio Capture [here](https://support.shinywhitebox.com/hc/en-us/articles/204161459-Installing-iShowU-Audio-Capture-Mojave-and-earlier-) and follow the steps on the website to install iShowU Audio Capture. **Make sure to download the right version for your OS (click on the Catalina one if you are running on Catalina)**

**Note** iShowU Audio allows Mac Users to route the audio from our computer into OBS, so people watching your stream

**2.**  Restart your Mac & accept security pop-up upon installing iShowU Audio successfully.

**3.** Check that you have installed iShowU Audio successfully by checking System Preference > Sound > Output and iShowU Audio shows up as one of your sound output options

![iShowU Audio Installed](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/iShowU%20Audio%20Installed.png?raw=true "iShowU Audio Installed Screenshot")

**4.** Click on the spotlight search (See 1 in the photo below), and type in "Audio MIDI Setup" (See 2 in the photo below). Open Audio MIDI Setup.

![Audio MIDI Setup](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Audio%20MIDI%20Setup.png?raw=true "Audio MIDI Setup Screenshot")

**5.** Create a multi output device that contains those two audio outputs. Click on the "+" button (See 1 in the photo below) and click on the drop-down "Create Multi-Output Device" (See 2 in the photo below). 
**Note** This will allow you to hear both your microphone and game/computer capture audio.

![Create Multiple Output Device](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Create%20Multiple%20Output%20Device.png?raw=true "Create Multiple Output Device Screenshot")

**6.** Select both the "Built-in Output"/"Your Own Sound Card" and iShowU Audio Capture


![Select Audio Output](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Select%20Audio%20Output.png?raw=true "Select Audio Output Screenshot")

**7.** Close Audio MIDI Setup's window

**8.** Go in System Preferences>Sound>Output, and make sure Output is set to <Streaming>
  
![Sound > Output](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Sound%3EOutput.png?raw=true "Sound > Output Screenshot")

### Capturing Audio Source for BOTH PC & Mac Users

**9.** Open OBS, and check if OBS is receiving mic's audio properly.

  1. Click on the setting button (labeled 1)
  2. Click on the drop-down menu named "Properties"

![Audio Properties](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Audio%20Properties.png?raw=true "Audio Properties Screenshot")

  3. Select where the mic audio is coming from by clicking the dropdown (Labeled 1)
  4. Select the mic (Labeled 2)
  5. Press OK (Labeled 3)

![Audio Properties Detail](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Audio%20Properties%20Detail.png?raw=true "Audio Properties Detail Screenshot")

**10.** Set up Advanced Audio Properties so audio from mic is outputting to both side of the headphone output.
        Follow the steps below.
        
  1. Click on the setting button (labeled 1)
  2. Click on the drop-down menu named "Advanced Audio Properties" (labeled 2)

![Advanced Audio Properties](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Advanced%20Audio%20Properties.png?raw=true "Advanced Audio Properties Screenshot")

  3. Make sure Mono is checked (Labeled 1)
  4. Press Close

![Advanced Audio Properties Detail](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Advanced%20Audio%20Properties%20Detail.png?raw=true "Advanced Audio Properties Detail Screenshot")

**11.** Rename mic audio

**12.** Add Audio Input Capture (your Mic audio) to Sources > Now your mic audio should be set up properly and you should be able to hear your mic through your headphone or Built-in Audio Ouput.

        
  1. Click on the '+' button (labeled 1)
  2. Click on the drop-down menu named "Audio Input Capture" (labeled 2)

![Add Mic Audio](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Add%20Mic%20Audio.png?raw=true "Add Mic Audio Screenshot")

  3. Click on 'Add Existing' (labeled 1) and select your mic 'SM7' in this case (labeled 2)
  4. Press 'OK' (label 3)

![Add Mic Audio Details](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Add%20Mic%20Audio%20Screenshot.png?raw=true "Add Mic Audio Details Screenshot")

**13.** Add Computer Audio Input Capture (your Computer Audio) to Sources

  1. Click on the '+' button (labeled 1)
  2. Click on the drop-down menu named "Audio Input Capture" (labeled 2)

![Add Computer Audio Input Capture](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Add%20Computer%20Audio%20Input%20Capture.png?raw=true "Add Computer Audio Input Capture Screenshot")
  
  3. Select 'Create new' and rename audio to 'Computer Audio' (labeled 1)
  4. Press 'OK' (labeled 2)

![Add Computer Audio Input Capture Detail](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Add%20Computer%20Audio%20Input%20Capture%20Detail.png?raw=true "Add Computer Audio Input Capture Detail Screenshot")

  5. Select 'iShowU Audio Capture'(labeled 1)
  6. Press 'OK' (labeled 2)

![Add Computer Audio Input Capture Detail 2](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Add%20Computer%20Audio%20Input%20Capture%20Detail2.png?raw=true "Add Computer Audio Input Capture Detail 2 Screenshot")

**14.** Test Computer Audio Input

  1. Click on the Apple Icon on the top left of the home screen (labeled 1)
  2. Go to System Preferences (labeled 2)
  3. Select 'Sound' (labeled 3)
  4. Click on 'Sound Effects' (labeled 4) and make sure 'Play sound effects through' is set to 'Screencap' (labeled 5)
  5. Click on one of the alert sounds, you should see the meter/sound bar under Computer Audio in OBS to be registering some audio. If the sound bar under Computer Audio is fluctuating up and down on OBS, it means your stream is registering your Computer Audio Output.


![System Preference Screenshot](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/System%20Preference%20Screenshot.png?raw=true "System Preference Screenshot")

![Sound](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Sound.png?raw=true "Sound Screenshot")

![Sound Testing](https://github.com/pazcharles02/OBS-and-Twitch-Livestreaming/blob/gh-pages/assets/images/Sound%20Testing.png?raw=true "Sound Testing Screenshot")


**Your audio is all set up and good to go for streaming.**
