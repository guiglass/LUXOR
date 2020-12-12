/*Eliminates padding, centers the thumbnail */

body, html {
padding: 0;
margin: 0;
text-align: center;
}

/* Styles the thumbnail */

a.lightbox img {
height: 150px;
border: 3px solid white;
box-shadow: 0px 0px 8px rgba(0,0,0,.3);
margin: 94px 20px 20px 20px;
}

/* Styles the lightbox, removes it from sight and adds the fade-in transition */

.lightbox-target {
position: fixed;
top: -100%;
width: 100%;
background: rgba(0,0,0,.7);
width: 100%;
opacity: 0;
-webkit-transition: opacity .5s ease-in-out;
-moz-transition: opacity .5s ease-in-out;
-o-transition: opacity .5s ease-in-out;
transition: opacity .5s ease-in-out;
overflow: hidden;
}

/* Styles the lightbox image, centers it vertically and horizontally, adds the zoom-in transition and makes it responsive using a combination of margin and absolute positioning */

.lightbox-target img {
margin: auto;
position: absolute;
top: 0;
left:0;
right:0;
bottom: 0;
max-height: 0%;
max-width: 0%;
border: 3px solid white;
box-shadow: 0px 0px 8px rgba(0,0,0,.3);
box-sizing: border-box;
-webkit-transition: .5s ease-in-out;
-moz-transition: .5s ease-in-out;
-o-transition: .5s ease-in-out;
transition: .5s ease-in-out;
}

/* Styles the close link, adds the slide down transition */

a.lightbox-close {
display: block;
width:50px;
height:50px;
box-sizing: border-box;
background: white;
color: black;
text-decoration: none;
position: absolute;
top: -80px;
right: 0;
-webkit-transition: .5s ease-in-out;
-moz-transition: .5s ease-in-out;
-o-transition: .5s ease-in-out;
transition: .5s ease-in-out;
}

/* Provides part of the "X" to eliminate an image from the close link */

a.lightbox-close:before {
content: "";
display: block;
height: 30px;
width: 1px;
background: black;
position: absolute;
left: 26px;
top:10px;
-webkit-transform:rotate(45deg);
-moz-transform:rotate(45deg);
-o-transform:rotate(45deg);
transform:rotate(45deg);
}

/* Provides part of the "X" to eliminate an image from the close link */

a.lightbox-close:after {
content: "";
display: block;
height: 30px;
width: 1px;
background: black;
position: absolute;
left: 26px;
top:10px;
-webkit-transform:rotate(-45deg);
-moz-transform:rotate(-45deg);
-o-transform:rotate(-45deg);
transform:rotate(-45deg);
}

/* Uses the :target pseudo-class to perform the animations upon clicking the .lightbox-target anchor */

.lightbox-target:target {
opacity: 1;
top: 0;
bottom: 0;
}

.lightbox-target:target img {
max-height: 100%;
max-width: 100%;
}

.lightbox-target:target a.lightbox-close {
top: 0px;
}


[< Main Page](https://github.com/guiglass/LUXOR/blob/gh-pages/index.md)

# Frequently Asked Questions


- **Is SteamVR required to run Luxor?**
  <details><summary>Yes, SteamVR is required.</summary>
 
	SteamVR is needed for tracker support and for interaction with props and scenes. *However many non-SteamVR HMDs and controllers are supported and can be used with SteamVR (Oculus, WMR, Kinect)*.
	  
	*it is possible to use some basic features on a PC with only a Oculus Quest 2 HMD and no SteamVR.*
  
   </details>



- **Can I use Luxor without a HMD?**
  <details><summary>Yes, Avatars may be connected to head trackers instead.</summary>
	It is possible to connect the avatar to a head tracker without the need for an HMD. This can be acomplished by configuring a tracker to function as a head tracker in the Tracer Setup menu:
	<p align="center">
	<a href="/img/tracker setup.png" target="_blank">
	 <img width="15%" height="15%" src="/img/tracker setup.png">
	</a>
	</p>
   </details>
- **Do I need trackers or can this be used with just controllers and an HMD?**
  <details><summary>Yes the avatar can be connected to only controllers and HMD and trackers are optional.</summary>
	There is basic locomotion for animating the avatar's lower body if no feet or hip trackers are preset or the avatar may be locked for standing or sitting in place. 
   </details>
- **Can I mix VR hardware such as valve index controllers with a Vive headset?**
  <details><summary>Yes, many VR HMDs and controllers are compatible.</summary>
	Users may mix controllers such as Knuckles, Vive wands, Oculus touch and WMR (using SteamVR).
   </details>
   
- **How do I interact with the menus?**

- **How do I record a mocap?**
Use the "Record Mocap" located button on the VR menu to start recording (alternatively you could use the spacebar hotkey)


- **How do I move around in Luxor? Can I do so while recording?**
  <details><summary>There are several ways users may move around in a scene.</summary>
	Some controls are located in the main menu for moving, rotating or scaling the avatar:
	<p align="center">
	<a target="_blank" href="/img/slew controls.png">
	 <img width="15%" height="15%" src="/img/slew controls.png">
	</a>
	</p>
	<p align="center">
	This panel is hidden during recording.
	</p>

	- Superhero fly mode may be enabled during recording, and when used in combination with raycast floor the avatar will remain attached to any floor but can be moved in the direction the user is pointing.
	<p align="center">
	<a target="_blank" href="/img/slew fly.png">
	 <img width="15%" height="15%" src="/img/slew fly.png">
	</a>
	</p>

	- The Sidekick app also has simplified controls for positioning the avatar in the scene remotely:
	<p align="center">
	<a target="_blank" href="/img/sidekick slew controls.png">
	 <img width="15%" height="15%" src="/img/sidekick slew controls.png">
	</a>
	</p>
   </details>
- **How do I export my scene to Blender?**
  <details><summary>Users can export the current recoreded scenes as blender files from the "export" panel.</summary>
	To export the current mocap and scene to Blender locate the *export* panel and enter a folder name where the files will be written and then pressing *export*:
	<p align="center">
	<a target="_blank" href="/img/panel ui export.png">
	 <img width="15%" height="15%" src="/img/panel ui export.png">
	</a>
	</p>

	- The menu in VR also provids an *export* panel and can be used to export the current scene to Blener files:
	<p align="center">
	<a target="_blank" href="/img/panel vr export.png">
	 <img width="15%" height="15%" src="/img/panel vr export.png">
	</a>
	</p>
   </details>  
- **How many trackers can I use in total?**
  <details><summary>Avatars may be connected to 11 points of tracking.</summary>
	Avatars may be connected to 11 points of tracking (hands, arms, elbows, feet knees, hip, chest, head). 
	<p align="center">
	<a target="_blank" href="/img/mocap_suit.jpg">
		<img width="15%" height="15%" src="/img/mocap_suit.jpg">
	</a>
	</p>
	
	And two auxilary trackers may be used for props and VR cameras.
   </details>
- **What versions of Unity and Blender should I be using?**
  <details><summary>Recomended versions are Unity 2019.4 and Blender 2.8+.</summary>
	- It's recomended to use Unity 2019.4 with the APS_SDK however other versions are compatible and the APS_SDK can be used with Unity 2018.4.20f1 (for backwards compatibility with vrchat). *The APS_SDK is not compatible with Unity 2020!*
	- Using Blender 2.8 is recomended, however 2.79 is mostly supported.
   </details>
- **Can I import a custom avatar into Luxor?**
  <details><summary>Yes, using the APS_SDK allows adding custom avatars.</summary>
	The APS_SDK allows adding avatars to Luxor using modles from either .fbx or .blend files: 
	<p align="center">
	<a target="_blank" href="https://youtu.be/oEwkhIr4ffw">
		<img width="15%" height="15%" src="http://i3.ytimg.com/vi/oEwkhIr4ffw/hqdefault.jpg">
	</a>
	</p>
	
   </details>
- **What types of avatars are supported?**
  <details><summary>Most avatars are supported so long as they can be configured as a standard humanoid in Unity.</summary>
	Using the APS_SDK almost any humanoid avatar can be added so long as the avatar can be configured as a standard humanoid in Unity.
   </details>
- **How do I make a prop that can be grabbed like the ones in Luxor?**

- **How do I import custom sets (worlds) into Luxor?**

- **How do I link the sidekick app and use it along with full body tracking?**

- **How do I link Luxor to Blender viewport in real time?**



- **Can Luxor be used offline?**
  <details><summary>Luxor is early access beta and requires verifying the activation token online.</summary>
  - Luxor is early access beta. When the program starts it requires verifying an activation token. After initially verifying activation no futher internet connection is required.
   </details>
- **What does the parental lock do?**
  <details><summary>It disables the ability to toggle mesh visiblity (clothing).</summary>
	Currently parental lock disables the ability to toggle mesh visiblity (clothing). But may be used in the future so users can lock adult props/avatars from loading or showing (for live streaming). 
   </details>

