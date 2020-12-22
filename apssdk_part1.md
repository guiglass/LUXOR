[< Main Page](index.md)

# Adding Custom Avatars (APS SDK Part 1)

<p align="center">
  <a href="img/aps sdk avatar builder main.png">
     <img width="50%"  src="img/aps sdk avatar builder main.png">
  </a>
</p>

**Installing the ASP SDK into a new Unity project**



Download [Unity 2019.4](https://unity3d.com/unity/whats-new/2019.4.16)
 - Unity 2020 is not supported!
 - The APS SDK is compatible with Unity 2018.4.20f1 for users who are also working with the VRCSDK.

Download [Blender](https://www.blender.org/download/)
 - Blender(2.79b) or (2.8 and above) are compatible but be consistent and keep in mind that Blender is not backwards compatible.
 - It is okay to create assets using Blender(2.79b) and later render them in Blender(2.8+).

Download [APS_SDK.unitypackage](https://github.com/guiglass/LUXOR/blob/gh-pages/APS_SDK.unitypackage?raw=true)
 - A copy of the *APS_SDK.unitypackage* can be found in the <sub><sup>%USERPROFILE%\AppData\LocalLow\Animation Prep Studios\LUXOR\Addons\APS SDK Unity</sup></sub> application folder.
 
After installing Unity and opeining Unity hub click on New project and ensure to have selected the proper Unity version from the dropdown:

<p align="center">
  <a href="https://raw.githubusercontent.com/guiglass/LUXOR/gh-pages/img/new%20project.png">
     <img width="50%" src="https://raw.githubusercontent.com/guiglass/LUXOR/gh-pages/img/new%20project.png">
  </a>
  <br>
  Create a new project.
</p>
<sub>You may optionally wish to stick to a standardized naming convention when creating new projects such as by prepending <b>APS_SDK_</b> to the begining of the project's name whenever creating a project to be used for building assets. The project name should also take into consideration if it will be used for creating an individual asset or batches of assets. For example, when I start a new Unity project for creating assets in batches I will typically name the project something similar to <b>APS_SDK_BATCH_MyCoolAvatars</b>.
</sub>
<br><br>

After clicking Create and allowing the project to load locate and add the APS_SDK.unitypackage asset into the project's *assets* folder:
<br>
<p align="center">
  <a href="img/import sdk.png">
     <img width="50%" src="img/import sdk.png">
  </a>
  <br>
  <sub><sup>Open the asset in Unity and click on Import.</sup></sub>
</p>
    Allow the package to decompress and be imported into the project:
  <br>
<p align="center">
  <a href="img/importing scripts.png">
     <img width="50%" src="img/importing scripts.png">
  </a>
</p>

If you see the Unity API Update Required click Go Ahead:
<br>
<p align="center">
  <a href="img/update unity api.png">
     <img width="50%" src="img/update unity api.png">
  </a>
</p>


<h1>Build an avatar from .fbx models.</h1>


<h1>Build an avatar from .blend models.</h1>

Locate the APS_SDK menu and select Avatar Builder:
<br>
<p align="center">
  <a href="img/avatar menu.png">
     <img width="50%" src="img/avatar menu.png">
  </a>
</p>


<br><br>
<p align="center">
  <a href="apssdk_part2.md">Adding Custom Props</a> (Part 2)
</p>
