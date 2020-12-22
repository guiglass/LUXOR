[< Main Page](index.md)

# Adding Custom Avatars 
**APS SDK Part 1**

<p align="center">
  <a href="img/aps sdk avatar builder main.png">
     <img width="50%"  src="img/aps sdk avatar builder main.png">
  </a>
</p>

## TLDR

It is possible to create avatars using <a href="#user-content-building-avatars-from-fbx">**.fbx**</a> files.<br>
It's also possible to create avatars using <a href="#user-content-building-avatars-from-blend">**.blend**</a> files with the Auto Avatar Importer



## Installing the ASP SDK into a new Unity project

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


The APS_SDK should now be installed in the new project. The next step is to build the actual humanoid avatar from a source model.
Thre are two types of files that can be supplied as a source models when using the APS_SDK. The first type is .fbx which after being added to the project it is also required to configure the asset as a Humanoid and ensure that Unity's Humanoid configuration is properly mapped to the correct bones.

<div id="building-avatars-from-fbx"></div>

## Avatars from **.fbx** models 

<p align="center">
  <a href="img/import fbx.png">
     <img width="50%" src="img/import fbx.png">
  </a>
  <br>
  <sub><sup>Move the humanoid .fbx into the new Unity project.</sup></sub>
</p>
    Allow the package to decompress and be imported into the project:
  <br>




<div id="building-avatars-from-blend"></div>

## Avatars from **.blend** models 

The APS_SDK includes an Auto Avatar Importer tool for building avatars from known conventions such as CC3 and Makehuman. To use the Auto Avatar Importer tool the user should save their humanoid source models as a .blend file. 

The Auto Avatar Importer is compatible with several starndard skeleton types and includes automation that simplifies the process of adding and importing avatars into the Unity editor and preparing them as an asset for LUXOR and final rendering in Blender.

There are some advantages to using the Auto Avatar Builder for importing an avatar from a .blend file. 
 * The Humanoid configuration in Unity is automatically mapped for all supported avatrar types.
 * Adds an auto-mapped <a href="img/visemeLinker.png">VisemeLinker</a> (lipsync component) using predefined templates *for some avatrar types*. 
 * Adds an auto-mapped <a href="img/facecapLinker.png">FacecapLinker</a> (facecap component) using predefined templates *for some avatrar types*. 
 * Adds assortments of auto-generated <a href="img/emotes.png">EmotionBuilder</a> (facial expressions components) using predefined templates *for some avatar types*.
 * Using .blend source models allows more flexibility when creating final renders and Blender scenes when using the SceneLoader. 

### Auto Avatar Importer Compatible Skeletons
|   Compatible Skeletons |  Emotes Templates  |  Facecap Templates  | Visemes Templates |
| :-------------| :-------------: | :-------------: |    :-------------: | 
|  CC3          |     Yes            |  Yes             | Yes             |
|  Fuse CC      |     Yes            |  Yes             | Yes             |
|  Makehuman    |     Yes            |  Yes            | Yes             |
|  Mixamo       |     Partial        |  Yes             | No             |
|  Rigify      |     No            |  No             | No             |
|  Daz3D (Gen2) |     No             |  No             | No             |
|  Daz3D (Gen3) |     No             |  No             | No             |

* Compatible Skeletons - Many character creator programs export their rigs with standard naming conventions.
* Emotes Templates - Addes <a href="img/emotes.png">EmotionBuilder.cs</a> components for setting up avatars with an assortment of default facial expressions.
* Facecap Templates - Adds a <a href="img/facecapLinker.png">FacecapLinker.cs</a> component and automaps known blendshapes to setup avatars for facial capture.
* Visemes Templates - Adds a <a href="img/visemeLinker.png">VisemeLinker.cs</a> component and automaps known blendshapes to setup avatars for microphone lipsync.



<br><br>
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
