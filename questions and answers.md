[< Main Page](https://github.com/guiglass/LUXOR/blob/gh-pages/index.md)

# Frequently Asked Questions


- **Can I use Luxor without a HMD?**
  - Yes, it is possible to connect the avatar to a head tracker without the need for an HMD. This can be acomplished by configuring a tracker to function as a head tracker in the Tracer Setup menu:
  <p align="center">
  <a href="/img/tracker setup.png">
     <img width="15%" height="15%" src="/img/tracker setup.png">
  </a>
  </p>
  
- **Can Luxor be used with only an HMD and controllers?**
  - Yes, there is basic locomotion for animating the avatar's lower body if no feet or hip trackers are preset or the avatar may be locked for standing or sitting in place. 
  
- **Can I mix VR hardware such as valve index controllers with a Vive headset?**
  - Yes, many VR HMDs and controllers are compatible such as Knuckles, Vive wands, Oculus touch and WMR (using SteamVR).
- **How do I move around in Luxor? Can I do so while recording?**
  - There are several ways users may move around in a scene. Some controls are located in the main menu for moving, rotating or scaling the avatar:
  <p align="center">
  <a href="/img/slew controls.png">
     <img width="15%" height="15%" src="/img/slew controls.png">
  </a>
  </p>
  <p align="center">
	This panel is hidden during recording.
  </p>

  
  - Superhero fly mode may be enabled during recording, and when used in combination with raycast floor the avatar will remain attached to any floor but move in the direction the user is pointing.
  <p align="center">
  <a href="/img/slew fly.png">
     <img width="15%" height="15%" src="/img/slew fly.png">
  </a>
  </p>
  
  - The Sidekick app also has simplified controls for moving the avatar remotely:
  <p align="center">
  <a href="/img/sidekick slew controls.png">
     <img width="15%" height="15%" src="/img/sidekick slew controls.png">
  </a>
  </p>
  
- **How do I export my scene to Blender?**
  - To export the current mocap and scene to Blender locate the *export* panel and enter a folder name where the files will be written and then pressing *export*:
  <p align="center">
  <a href="/img/panel ui export.png">
     <img width="15%" height="15%" src="/img/panel ui export.png">
  </a>
  </p>
  
  - The menu in VR also provids an *export* panel and can be used to export the current scene to Blener files:
  <p align="center">
  <a href="/img/panel vr export.png">
     <img width="15%" height="15%" src="/img/panel vr export.png">
  </a>
  </p>
- **How many trackers can I use in total?**
  - Avatars may be connected to 11 points of tracking (hands, arms, elbows, feet knees, hip, chest, head). And two auxilary trackers for props or cameras
  <p align="center">
  <a href="/img/mocap_suit.jpg">
     <img width="15%" height="15%" src="/img/mocap_suit.jpg">
  </a>
  </p>
- **What versions of Unity and Blender should I be using?**
  - It's recomended to use Unity 2019.4 with the APS_SDK however other versions are compatible and the APS_SDK can be used with Unity 2018.4.20f1 (for backwards compatibility with vrchat).
  - Using Blender 2.8 is recomended, however 2.79 is mostly supported.
  
- **Can I import a custom avatar into Luxor?**
  - Yes, the APS_SDK allows adding avatars to Luxor using modles from either .fbx or .blend files.
  
- **What types of avatars are supported?**
	Using the APS_SDK almost any humanoid avatar can be added so long as the avatar can be configured as a standard humanoid in Unity.

- **How do I make a prop that can be grabbed like the ones in Luxor?**

- **How do I import custom sets (worlds) into Luxor?**

- **How do I link the sidekick app and use it along with full body tracking?**

- **How do I link Luxor to Blender viewport in real time?**

- **Can Luxor be used offline?**
  - Luxor is early access beta. When the program starts it requires verifying an activation token. After initially verifying activation no futher internet connection is required.
  
- **What does the parental lock do?**
  - Currently parental lock disables the ability to toggle mesh visiblity (clothing). But may be used in the future so users can lock adult props/avatars from loading or showing (for live streaming). 
