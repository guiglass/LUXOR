[< Main Page](https://github.com/guiglass/LUXOR/blob/gh-pages/index.md)

# Frequently Asked Questions


- Q: **Can I use Luxor without a HMD?**
  - Yes, it is possible to connect the avatar to a head tracker without the need for an HMD. This can be acomplished by configuring a tracker to function as a head tracker in the Tracer Setup menu:
  <p align="center">
  <a href="/img/tracker setup.png">
     <img width="15%" height="15%" src="/img/tracker setup.png">
  </a>
  </p>
  
- Q: **Can Luxor be used with only an HMD and controllers?**
  - Yes, there is basic locomotion for animating the avatar's lower body if no feet or hip trackers are preset or the avatar may be locked for standing or sitting in place. 
  
- Q: **Can I mix VR hardware such as valve index controllers with a Vive headset?**
  - Yes, many VR HMDs and controllers are compatible such as Knuckles, Vive wands, Oculus touch and WMR (using SteamVR).
- Q: **How do we move around in Luxor? Can we do so while recording?**
  - There are several ways users may move around in a scene. Some controls are located in the main menu for moving, rotating or scaling the avatar:
  <p align="center">
  <a href="/img/slew controls.png">
     <img width="15%" height="15%" src="/img/slew controls.png">
  </a>
  </p>
  <p align="center">
	This panel is hidden during recording.
  </p>

  
  Superhero fly mode may be enabled during recording, and when used in combination with raycast floor the avatar will remain attached to any floor but move in the direction the user is pointing.
  <p align="center">
  <a href="/img/slew fly.png">
     <img width="15%" height="15%" src="/img/slew fly.png">
  </a>
  </p>
  
  The Sidekick app also has simplified controls for moving the avatar remotely:
  <p align="center">
  <a href="/img/sidekick slew controls.png">
     <img width="15%" height="15%" src="/img/sidekick slew controls.png">
  </a>
  </p>
  
- Q: **How do I export my scene to Blender?**
  - To export the current mocap and scene to Blender locate the *export* panel and enter a folder name where the files will be written and then pressing *export*:
  <p align="center">
  <a href="/img/panel ui export.png">
     <img width="15%" height="15%" src="/img/panel ui export.png">
  </a>
  </p>
  
  The menu in VR also provids an *export* panel and can be used to export the current scene to Blener files:
  <p align="center">
  <a href="/img/panel vr export.png">
     <img width="15%" height="15%" src="/img/panel vr export.png">
  </a>
  </p>
- Q: **How many trackers can I use in total?**
  - Avatars may be connected to 11 points of tracking (hands, arms, elbows, feet knees, hip, chest, head). And two auxilary trackers for props or cameras
  <p align="center">
  <a href="/img/mocap_suit.jpg">
     <img width="15%" height="15%" src="/img/mocap_suit.jpg">
  </a>
  </p>
- Q: **What versions of Unity and Blender should I be using?**

- Q: **Can I import a custom avatar into Luxor?**

- Q: **What types of avatars are supported?**

- Q: **How do I make a prop that can be grabbed like the ones in Luxor?**

- Q: **How do we import custom sets (worlds) into Luxor?**

- Q: **How do we link the sidekick app and use it along with full body tracking?**

- Q: **How do we link Luxor to Blender viewport in real time?**

- Q: **Can Luxor be used offline?**
  - Luxor is early access beta. When the program starts it requires verifying an activation token. After initially verifying activation no futher internet connection is required.
  
- Q: **What does the parental lock do?**
  - Currently parental lock disables the ability to toggle mesh visiblity (clothing). But may be used in the future so users can lock adult props/avatars from loading or showing (for live streaming). 
