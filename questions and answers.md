[< Main Page](index.md)

# Frequently Asked Questions

- **Is SteamVR required to run LUXOR?**
  <details><summary>Yes, SteamVR is required.</summary>
	🍎 SteamVR is needed for tracker support and for interaction with props and scenes. *However many non-SteamVR HMDs and controllers are supported and can be used with SteamVR (Oculus, WMR, Kinect)*.
	  
	*it is possible to use some basic features on a PC with only a Oculus Quest 2 HMD and no SteamVR.*
  
   </details>

- **Can I use LUXOR without a HMD?**
  <details><summary>Yes, Avatars may be connected to head trackers instead.</summary>
	🍎 It is possible to connect the avatar to a head tracker without the need for an HMD. This can be acomplished by configuring a tracker to function as a head tracker in the Tracer Setup menu:
	<p align="center">
		<img width="15%" height="15%" src="/img/tracker setup.png"/>
	</p>
   </details>
- **Do I need trackers or can this be used with just controllers and an HMD?**
  <details><summary>Yes the avatar can be connected to controllers and HMD only, trackers are optional.</summary>
	🍎 There is basic locomotion for animating the avatar's lower body if no feet or hip trackers are preset or the avatar may be locked for standing or sitting in place. 
   </details>
- **Can I mix VR hardware such as valve index controllers with a Vive headset?**
  <details><summary>Yes, many VR HMDs and controllers are compatible.</summary>
	🍎 Users may mix controllers such as Knuckles, Vive wands, Oculus touch and WMR (using SteamVR).
   </details>
   
- **How do I interact with the menus?**

- **How do I record a mocap?**
  <details><summary>Click the "Record Mocap" button located on the VR menu.</summary>
	🍎 Click the "Record Mocap" located on the VR menu to start recording (alternatively you could use the spacebar hotkey)
   </details>

- **How do I move around in LUXOR? Can I do so while recording?**
  <details><summary>There are several ways users may move around in a scene.</summary>
	🍎 Some controls are located in the main menu for moving, rotating or scaling the avatar:
	<p align="center">
		<img width="15%" height="15%" src="/img/slew controls.png">
	</p>
	<p align="center">
	This panel is hidden during recording.
	</p>

	- Superhero fly mode may be enabled during recording, and when used in combination with raycast floor the avatar will remain attached to any floor but can be moved in the direction the user is pointing.
	<p align="center">
		<img width="15%" height="15%" src="/img/slew fly.png">
	</p>

	- The Sidekick app also has simplified controls for positioning the avatar in the scene remotely:
	<p align="center">
	 <img width="15%" height="15%" src="/img/sidekick slew controls.png">
	</p>
   </details>

- **<div id="target1"> </div>How do I export my scene to Blender?**
  <details><summary>Users can export the current recoreded scenes as blender files from the "export" panel.</summary>
	🍎 To export the current mocap and scene to Blender locate the *export* panel and enter a folder name where the files will be written and then pressing *export*:
	<p align="center">
	 <img width="15%" height="15%" src="/img/panel ui export.png">
	</p>

	- The menu in VR also provids an *export* panel and can be used to export the current scene to Blener files:
	<p align="center">
		<img width="15%" height="15%" src="/img/panel vr export.png">
	</p>
   </details>  
- **How many trackers can I use in total?**
  <details><summary>Avatars may be connected to 11 points of tracking.</summary>
	🍎 Avatars may be connected to 11 points of tracking (hands, arms, elbows, feet, knees, hip, chest, head). 
	<p align="center">
		<img width="15%" height="15%" src="/img/mocap_suit.jpg">
	</p>
	
	And two auxilary trackers may be used for props and VR cameras.
   </details>
- **What versions of Unity and Blender should I be using?**
  <details><summary>Recomended versions are Unity 2019.4 and Blender 2.8+.</summary>
	🍎 It's recomended to use Unity 2019.4 with the APS_SDK however other versions are compatible and the APS_SDK can be used with Unity 2018.4.20f1 (for backwards compatibility with vrchat). *The APS_SDK is not compatible with Unity 2020!*
	- Using Blender 2.8 is recomended, however 2.79 is mostly supported.
   </details>
- **Can I import a custom avatar into LUXOR?**
  <details><summary>Yes, using the APS_SDK allows adding custom avatars.</summary>
	The APS_SDK allows adding avatars to LUXOR using modles from either .fbx or .blend files: 
	<p align="center">
		<img width="15%" height="15%" src="http://i3.ytimg.com/vi/oEwkhIr4ffw/hqdefault.jpg">
	</p>
	
   </details>
- **What types of avatars are supported?**
  <details><summary>Most avatars are supported so long as they can be configured as a standard humanoid in Unity.</summary>
	🍎 Using the APS_SDK almost any humanoid avatar can be added so long as the avatar can be configured as a standard humanoid in Unity.
   </details>
   
- **How do I make a prop that can be grabbed like the ones in LUXOR?**

- **How do I import custom sets (worlds) into LUXOR?**

- **How do I link the sidekick app and use it along with full body tracking?**

- **How do I link LUXOR to Blender viewport in real time?**

- **Can LUXOR be used offline?**
  <details><summary>Yes, APS LUXOR may be used offline and does not require any internet connection.</summary>
	🍎 LUXOR is an early access beta and currently does not require any connection to the internet.
   </details>
- **What does the streamer mode do?**
  <details><summary>It disables some features and prevents loading any assets marked with NSFW.</summary>
	🍎 This feature is still under active development but currently streamer mode is enabled by default. By checking will disable some features that might be considered unsafe for livestreaming and prevents loading any assets marked with NSFW option when they were created in the APS_SDK.</details>

- **Is LUXOR a plugin for Blender?**
  <details><summary>No, APS LUXOR is a game/tool that can record exports the animations and avatars as Blender friendly files.</summary>
	🍎 It's not exactly a plugin, it's a game/tool that can record mocap using VR hardware and then exports the animations and avatars as Blender friendly files into their own 'project folder'. But there is a SceneLoader.blend that is used to import those files and automatically set up the blender scene so as to have things ready to render in minutes.
</details>


