
<h1 style="line-height:2;"><p align="center"><a href="https://nexplayersdk.com/unreal-player-sdk-demo/" target="_blank"><img  src="https://github.com/NexPlayer/NexPlayer_Unity_Plugin/blob/master/resources/Button Demo_2.png" width="23%" height="10%" alt="Unity video player" align="right"></img></a>
<a align=right href="https://nexplayersdk.com/unreal-player-sdk-demo/" target="_blank"><img src="Source/Images/last.png" width="100%" height="100%" ></a>
</p></h1>
</br>

<p align="center"><img  src="Source/Gifs/Edited Fortnite GIF.gif" width="100%" height="100%" alt="Cube Demo" align="center"></img>
</p>
<br>

NexPlayer™ for Unreal Engine is a video streaming plugin that enables **HLS & DASH streaming** on **Android**, **iOS**, **HTML5** / **Web** and **Windows** apps and games. NexPlayer supports Unreal Pixel Streaming. It allows to create interactive video content within Unreal Engine project and stream it to any device with Pixel Streaming.

NexPlayer will be available for **more platforms** soon, stay tuned.


This repository contains the NexPlayer™ for Unreal feature list as well as an installation guide. If you want to try a demo and see the full documentation, please contact us at our [website](https://nexplayersdk.com/unreal-player-sdk/).

Supported UNREAL ENGINE VERSIONS: UE4.22, 4.23, 4.24, 4.25, 4.26, 4.27, & UE5/Unreal Engine 5.

<br>
<p align="center">
 <img  src="Source/Gifs/2020_11_17.gif" width="600px" height="319px" alt="Cube Demo" align="center"></img>
</p>
<br>

## Table of Contents

* **[Features](#features)**  

* **[Supported Platforms](#supported-platforms)**

* **[Demo Installation Guide](#demo-installation-guide)**
 
 <br> 
<p align="center"><b>Live streaming inside Unreal games and apps</p>
<p align="center"><img  src="Source/Gifs/Edited tvshow GIF.gif" width="600px" height="319px" alt="Cube Demo" align="center"></img>
<p align="center"><b>Stream Amazon IVS inside Unreal Engine</p>
<p align="center"><img  src="Source/Gifs/unreal_AWS_IVS.gif" width="600px" height="319px" alt="Cube Demo" align="center"></img>

<br>


<p style="margin-left:auto;margin-right:auto" width="300px" align="left">Our Unreal video player plugin enables the introduction of new exciting use cases inside your Unreal games, such as concerts, video items related to the game or new metaverse experiences. </p>

## Features

The NexPlayer™ for Unreal Engine video streaming player is developed entirely **in-house**, making it fully customizable to implement any desired functionality. Don't hesitate to contact us if you need specific features not supported yet.

We support the following features:

<table>
 <tbody style="text-align:center;">
   <tr>
     <td valign="top" style="text-align:center;">
         <p style="max-width:100%;"><b>Overview</b></p>
     </td>
     <td>
       <ul>
       <li>HLS & DASH Streaming with ABR (Adaptive Bitrate)</li>
       <li>Amazon IVS</li>
       <li>Unreal Pixel Streaming</li>
       <li>Timed Metadata</li>
       <li>ID3 Tag</li>
       <li>Ad Insertion</li>
       <li>360 Video Playback and Virtual Reality (VR)</li>
       <li>Windows Editor (C++ & Blueprint)</li>
       <li>Up to 8K (UHD) Resolution</li>
       <li>Up to 60 Frames Per Second (FPS)</li>
       <li>Rendering Videos on 3D Objects</li>
       </ul>
     </td>
        <tr>
            <td valign="top" style="text-align:center;">
            <p style="max-width:100%;"><b>Basic Features</b></p>
     </td>
     <td>
       <ul>
        <li>Open Video Content</li>
        <li>Play / Pause</li>
        <li>Stop</li>
        <li>Loop</li>
        <li>AutoPlay</li>
        <li>Mute</li>
        <li>Close</li>
       </ul>
     </td>
     </tr>
   </tr>
 </tbody>
</table>

## Supported Platforms

| Platform | Supported Graphics APIs | HLS | DASH | 
| :-----:| :-----:| :-----:| :-----:| 
| Android  | OpenGLES2, OpenGLES3 | :heavy_check_mark: | :heavy_check_mark: | 
| iOS  | Metal | :heavy_check_mark: | :heavy_check_mark: | 
| Windows | DirectX11 / DirectX12 | :heavy_check_mark: | :heavy_check_mark: | 
| Android VR  | OpenGLES2, OpenGLES3 | :heavy_check_mark: | :heavy_check_mark: |
| HTML5  | WebGL 1.0 / WebGL 2.0 | :heavy_check_mark: | :heavy_check_mark: |

## Demo Installation Guide

### 1) Plugin Import

<p> Close your Unreal project if it is open. </p>

<p> Unzip the NexPlayerUnreal SDK (NexPlayer Demo Project) and copy the folder <i>NexPlayerUnreal/Plugins/NexPlayerUnreal</i> (NexPlayer Unreal Plugin) inside of the Plugins folder of your project. <br/> If you don't have a Plugins folder in your project, create one: </p>
<img  src="Source/Images/QuickStart/Step_02.PNG" width="80%" height="80%" alt="Quickstart_Step_2" align="center"></img><br>


<p> Open the project and open the Plugins Window:</p>
<img  src="Source/Images/QuickStart/Step_03.png" width="80%" height="80%" alt="Quickstart_Step_3" align="center"></img><br>


<p> Scroll all the way down to the Project section and under the Video category, select NexPlayerUnreal and check Enabled:</p>
<img  src="Source/Images/QuickStart/Step_04.png" width="80%" height="80%" alt="Quickstart_Step_4" align="center"></img><br>


<p> A yellow prompt will pop-up asking you to restart the editor, press the Restart Now button: </p>
<img  src="Source/Images/QuickStart/Step_05.png" width="80%" height="80%" alt="Quickstart_Step_5" align="center"></img><br>


<p> Unreal Engine will compile the plugin and open the project, with the plugin fully imported. </p>

### 2) Video Setup

<p> Add to the scene some basic actor where the rendering will occur. It needs to have the UVs properly set. It's recommended to use a Plane or Shape cube (the regular primitive cube won't work because of it's UVs): </p>
<img  src="Source/Images/QuickStart/Step_06.png" width="80%" height="80%" alt="Quickstart_Step_6" align="center"></img><br>

<p> Scale the Actor to match the desired video screen ratio (generally 16:9).
On the bottom right corner of the Content Browser, press View Options and make sure Show Plugin Content: </p>
<img  src="Source/Images/QuickStart/Step_07.png" width="80%" height="80%" alt="Quickstart_Step_7" align="center"></img><br>

<p> Add the BP_NexPlayer Actor located in NexPlayerUnreal Content/Blueprints to the scene: </p>
<img  src="Source/Images/QuickStart/Step_08.png" width="80%" height="80%" alt="Quickstart_Step_8" align="center"></img><br>

<p> Select the BP_NexPlayer Actor and set the stream URL in the Details tab: </p>
<img  src="Source/Images/QuickStart/Step_09.png" width="80%" height="80%" alt="Quickstart_Step_9" align="center"></img><br>

<p> Add one element to Target Actors in the Details tab and reference the Actor you added before: </p>
<img  src="Source/Images/QuickStart/Step_10.png" width="80%" height="80%" alt="Quickstart_Step_10" align="center"></img><br>

<p> Play the scene, and you will see your video rendering on the target Actor: </p>
<img  src="Source/Gifs/GuideTest.gif" width="80%" height="80%" alt="Quickstart_Step_11" align="center"></img><br>

-------------------


## Contact
[unreal.support@nexplayer.com](mailto:unreal.support@nexplayer.com)
<br>+34 914 184 356
<br>See you also at trade shows around the world!
<p align="center">
 <img  src="Source/Images/GDC.jpg" width="50%" height="50%"></a>
</p> 
<br>
<sub><sup>Android media player plugin for Unreal Engine, Unreal marketplace, Windows media player plugin for Unreal Engine, Media Player plugin for Unreal Engine, Stream live performances and media into your Unreal project, HLS and DASH streaming within Unreal Engine, Unreal Engine Video Streaming, UE4 live streaming, UE5 live streaming, web3, real-time 3D world, Unreal Engine 4 HTML5, NFT, cryptocurrency, web3 gaming and entertainment, blockchain, Electra Media Player, Media player plugin for Unreal, Unreal Engine 4, Unreal web, UE4, Unreal Engine 5, Epic games, Oculus Quest, Oculus Quest 2, Meta Oculus, Gear VR, HTC Vive, Google Cardboard, Daydream, Pico Goblin & Neo, electronic dance music, metaverse, AR, VR, XR, Amazon Interactive Video Service, Amazon IVS Unreal, timed metadata, embed metadata, metadata, ID3 tags, timestamps, Azure PlayFab, webbrowser, webGL, HTML5, unreal web player, unreal html5 video, Twitch.</sub><sup>
 
