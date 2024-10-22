# THE CAR SHOWROOM!
THE CAR SHOWROOM is a space where you can showcase your cars, featuring preset cameras, animations, and more.

## Table of Contents
* [Requirements](#Requirements)
* [Features](#Features)
* [Installation](#Installation)
  * [Game Setup](#Game-Setup)
  * [Car Installation](Car-Installation)
* [Important](#Important)
  * [Hotkey](#Hotkey)
  * [Properties Formats](#Properties-Formats)
* [Create a Camera](#How-to-create-camera)
  * [Methods 1](#Methods-1)
  * [Methods 2](#Methods-2)
* [Create a Animation](##Create-a-animation)
  * [Startings](#Startings)
  * [The-Scripts](#The-scripts)
  * [Other details](#Other-details)
   

## Requirements
- Have bough "THE CAR SHOWROOM" in Nova Tech Store

## Features
- Camera Preset
- Animation Preset
- Car Manager
- DataStore

## Important
### Hotkey
|Hotkey|Default|Additional|
|:-|:-|:-|
|Hide all UI|H|Configurable in the settings module.|
|Play/Stop|J|Configurable in game.|
|Pause/Resume|P|Configurable in game.|
|Free Cam Mode|Shift + P|Free Camera Mode of Roblox.|
### Properties Formats
|Name|Format|Default|Additional|
|:-|:-|:-|:-|
|Speed|A number|0.05|(Only for the View360 animation.)|
|Time|A number|1|(Time of the animation.)|
|Delay|A number|1|(Delay between reach repeat)|
|Camera Height|A number|5|Camera Height is for adjusting the view when swiping over big or small cars.|
|Camera Front-Back|A number|5|Camera Front-Back is for adjusting the view when swiping over big or small cars.|
|Camera Right-Left|A number|5|Camera Right-Left is for adjusting the view when swiping over big or small cars.|
|RepeatCounts|A number|0|(How much time this will repeat|
|Offset|x,y,z|0,2,15|(Only for View360 animation)|
|Hotkey|A single letter|X|X|

## Installation
### Game Setup:
- Open the .rbxl file.
- Publish the game.
- Go to Settings > Security.
- Enable HTTP Requests.
- Enable Studio Access to API Services.
- Join the game once, then leave.
### Car Installation:
- Get your car in the game.
- Set the car's position to (0, 0, 0) and raise it so the wheels aren't embedded in the ground.
- Put the car in game.ReplicatedStorage.Cars
- Do this for all your car and its done!

## How to create a Camera
### Methods 1:
- I created a plugin that places a camera at your current position in the studio,
- For get it go in ServerStorage save the "Plugin" as a local plugin,
- Position yourself where you want the camera to be placed,
- Click on the button in the plugin tabs or use a custom shortcut (File > Advanced > Customize Shortcuts). Search for "Create a Part" and assign a shortcut, for example, (Shift + Ctrl + C).
- Then you can rename the part ("New Camera") in the CamFolder to anything you want.
### Methods 2:
- Add a part in cam Folder,
- Rename it to anythings you want,
- Anchor the part,
- **Option 1:**
- Place the part where you want the camera to be placed.
- **Option 2:**
- Position yourself where you want the camera to be placed,
- Copy CFrame of Camera in Workspace (Workspace.Camera) A CFrame should be like this ({posX, posY, posZ}, {orientationX, orientationY, orientationZ})
- Paste the CFrame into the CFrame property of the part.

## Create a Animation
### Startings:
- Create a folder with the animation name in (CamFolder.Animated[YourAnimationName])
- Next, create "Waypoints" using the same method as "How to create a camera" (Waypoints are the points where the camera will pass).
- Name these waypoints (1, 2, 3, 4, 5, etc.) and place them in the folder you just created (They are in CamFolder with name "New Camera").

### The scripts:
Get the template I placed in ServerStorage named "TemplateAnimation," then follow the instructions from lines 3 to 9.

### Other details
You can create your own custom animation using your own methods, but just make sure that the module is placed in `game.ReplicatedStorage.Module.AnimationManager.Animation`.

