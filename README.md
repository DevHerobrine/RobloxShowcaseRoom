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
* [Create a Animation](#Create-a-animation)
  * [Startings](#Startings)
  * [The-Scripts](#The-scripts)
* [Map Manager](#Map-Manager)
  * [How import your Map?](#How-import-your-Map)

## Requirements
- Have bough "THE CAR SHOWROOM" in Nova Tech Store

## Features
- Camera Preset
- Animation Preset
- Car Manager
- Map Manager
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
|Speed|A number|0.2|(Only for the View360 animation.)|
|Time|A number|3|(Time of the animation.)|
|Delay|A number|0|(Delay between reach repeat)|
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
- Before creating waypoints, make sure you know what you want. You have two options:
  1. The camera will pass through all waypoints.
  2. The camera will move from waypoint 1 to waypoint 2, then from waypoint 3 to waypoint 4.
- Next, create "Waypoints" using the same method as "How to create a camera".
- Name these waypoints (1, 2, 3, 4, 5, etc.) and place them in the folder you just created (They are in CamFolder with name "New Camera").

### The scripts:
If you use option 1, then in ServerStorage.TemplateAnimation, choose TemplateAnimation1. If you use option 2, choose TemplateAnimation2. 
Next, follow the instructions in the module.

## Map Manager
### How import your Map?
- First if you don't have already it get the plugins
- For get it go in ServerStorage save the "Plugin" as a local plugin,
- Next go on the maps your want imports, and press copy Ligthings,
- Place the folder that just created named "LightingSettings", in the MapsFolder like that: ![image](https://github.com/user-attachments/assets/b320bafc-40aa-49c3-9cf8-fe453d294926)
- Copy your maps, paste it in ReplicatedStorage.Maps
- Remember that the cars are at position 0,0,0 so check if your maps are positioned correctly

