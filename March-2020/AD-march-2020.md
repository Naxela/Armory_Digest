![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/1.jpg)

## Armory Digested - March 2020

Welcome to the latest edition of the Armory Digested. Chewing the changes for you, so you don't have to dig source code

---

### What is this?

I've been thinking a bit about that it's been quiet on the forums, and that people have begun wondering if the engine is dead. At first glance, it might seem like there isn't happening much - Especially if you just happened to smack down into the forums here, maybe comparing it to other engines, and finding out that the last release note is from september last year. Maybe you'll even begin to think the engine and/or it's community is dead, but while it might not seem like a lot of stuff happens, it's a small but growing community.

Another part of it, is that it's largely a one-man project as of now, covering everything from development (Armory/Iron), bug-fixing, documentation and social-media - But being an open-source project where everyone is free to participte it doesn't necessarily have to be that way. Everyone is welcome to chip in, whether with development, documentation, showcasing features or in this case a brief roundup of what's happening in the Armory community.

---

### News

- Armory2020 Plans - (https://github.com/armory3d/armory/issues/1545) - These plans covers moving on to the newer Graphics5 (G5) API in Kinc, implementing raytracing in dynamic scenes, move low-level parts from Haxe to C for better multithreading and performance. You will still be able to write your traits in Haxe. Web-deployment (HTML5) will also still be supported.


- Armorpaint now running on Android through Kinc+Krom. Progress with this also means progress for Armory3D and the engines capabilities on the Android platform.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/2.jpg)

- Armorpaint awarded a well-deserved megagrant from Epic Games.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/3.jpg)

---

### Armory3D Changes (Since 2020.1)

*This section only covers changes from january. For an overview of features since 0.5, see the section at the bottom.*

- GetWorld node - Gives you a vector based on the world transform.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/4.jpg)

- Trait detail view for the debug console - Now shows a tree view outliner, and lists the traits connected to the selected object.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/5.jpg)

- Postprocessing nodes - Now allows for realtime editing of postprocessing values, such as bloom, SSR, ambient occlusion and also includes a large set of colorgrading options.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/6.jpg)

- Canvas Font size
- Exported asset names for trait properties
- getCanvas() function for canvasScript
- Better property recognition
- Better handling for duplicate objects
- Exposed postprocessing uniforms
- Plenty of fixes

[See the commits here](https://github.com/armory3d/armory/compare/20.01...master)

Contributors:
- Lubos, MoritzBrueckner, BlackGoku36, N8n5h, Sandy1000, Blackno666, Sanva, philipmduarte, Naxela

---

### Armorpaint Changes (Since 0.7)

- Cached UI draws
- Zoom operators
- Improved material export
- Greyscale mask
- Browser
- Opacity painting
- Support for network paths
- UV map of selected objects
- Layer groups, can be saved and drag-reordered
- Material preview in browser
- Stubs for exporting mesh (.obj) with displacement
- Improved pen radius scaling
- Copyable text
- Improved touch input
- Base layer masking and improved handling
- Raytrace builder
- Raytracing depth of field
- Alpha channel export
- Vertex color bakes
- macOS builds are signed
- Vertex color support
- Configuration saving
- Configuration initialization improved
- And more!

[See the commits here](https://github.com/armory3d/armorpaint/compare/20.01...master)

[See the release notes here](https://armorpaint.org/notes.html)

---

### Community Updates

- Did you read this months brand new Armory digest? Read it on the Armory forum!
- Alternatively you can [read them on Github](https://github.com/Naxela/Armory_Digest) as they're being compiled
- Want help write or want to showcase something you've made? Feel absolutely free to contribute
here
- Not the best writer? Don't worry, we'll fix your text before published on the forum
- Or better yet, discuss and make new threads about things you find interesting related to Armory!

---

### Featured example

*This months random example in focus*

**file_write** is an example that shows you how to write files from Krom. The way it works is that it converts a json object to bytes, and saves that information to a file in a specified location.
This example shows you one of the various ways to save your game data to a file. 

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/7.jpg)

---

### Featured tutorial
- Hologram Effect by Armory Blender (https://www.youtube.com/watch?v=ceRJtU_6TXY)

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/8.jpg)

---

### Showcase spotlights

- Active Games has Offroad Mania on steam! (https://store.steampowered.com/app/1222040/Offroad_Mania/)

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/9.jpg)

- Simonrazer made a multiplayer FPS demo (https://www.youtube.com/watch?v=-Iye7ALplCg)

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/10.jpg)

- m_entent has progress on Grease pencil (Screencap from Discord)

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/11.jpg)

---

### Support Armory and the ecosystem
- Lubos @ Armory3D, Armorpaint, Iron - https://armory3d.org/fund.html
- Robert @ Kha, Kinc, Krom - https://www.patreon.com/RobDangerous


### Visit the discord
- https://discord.gg/Vymh2r 


---
---
---
# Changes between Armory 0.5 and Armory 2020

A lot of stuff has happened with Armory. Since the last officially announced Armory release there's been a whopping 800+ commits to the Armory repo since version 0.5 with just about 35,000 lines of codes changed (additions and deletions)! That's a lot!

## Bigger features:

## Armory now comes as a Blender addon
Armory is now mainly a Blender 2.8 addon rathar than a fully packaged solution. This allows you to use whatever flavor of Blender (such as the fasterE-Cycles if you do a lot of texture baking). Installation is as easy as ever:

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/12.jpg)

## Voxel AO instead of Voxel GI - Voxel GI will be reworked into raytracing
A few users might have noticed that using Voxels as a way of doing Global Illumination have now been removed. Instead, focus will now be put on implementing raytracing technologies into Armory. This is currently being tested out in Armorpaint (Check out the DXR releases).

In the meantime, Voxel for Ambient Occlusion will still be available as a solution for achieving great ambient shadows.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/13.jpg)

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/15.jpg)

## New water, weather and terrain
While the old water and clouds looked great, the new systems looks even better! An overhaul of the weather system, that includes better water management, water refraction and cloud radiance has been implemented to make your nature scenes even better. On top of that, the new terrain system uses heightmaps, sectors and streaming while still working with physics.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/14.jpg)

## Krom patching
As a result of the default way of providing Armory builds is SDK releases, this means the Blender builds with the integrated V8/Node based viewports aren't there anymore. Instead, the default way of getting real-time output is by turning on Krom Live Patching. This provides the separate Krom window with realtime changes.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/15.gif)

## Eye adaption
Eye adaption / Auto-exposure with histogram have been reworked, and now allows the exposure to transition gradually to the light-settings of various environments. 

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/16.jpg)

## Haxe compilation server
By default, Armory now uses a multi-threaded Haxe-based compilation server in the never ending quest for more speed!

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/17.jpg)

## Clustered rendering
More performance is good performance! - With the introduction of recent shader models and improved rendering possibilities, Clustered shading/rendering is a way of providing fast high-fidelity graphics.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/18.jpg)

## Reflection Probes and Planes
Work on realtime reflection probes and plane have been done. Reflection Probes and Reflection Planes allows for much higher quality reflection than what Screen-Space Reflections can provide, and at all angles even outside the screen-space.

![](https://github.com/Naxela/Armory_Digest/blob/master/March-2020/img/19.jpg)

New examples and templates:
- All reworked into B.28
- Third person terrain
- Race Track
- Platformer
- Mesh Import
- Basic Terrain
- Volumetric
- Render to Texture
- Spawn from Scene

## Git-wise features:
- Exposed draw-order
- Asset destination
- Shader parameters
- Geometry Backfacing socket
- Khamake threads
- Soft Body solver iterations
- Reflection planes
- Reflection probes
- Debug tilde key
- Spawn object node
- CallFunction => CallHaxe => CallFunction (Can now call functions as well) :: Node functions!
- CallStaticFunction => CallHaxeStaticNode
- Parse color writes
- Fixes to onTimer node
- Canvas SetLocation Node
- Runtime Shader Generation
- Allow arbitrary node categories
- Logic nodes sorted alphabetically
- Gravity toggle node
- Support for Continuous Collision Detection for Rigid Bodies
- Shadow Cubemap exposed
- Colorspace are now read (SRGB and Non-Color)
- Runtime configurations
- Error when sockets don't match
- Set Camera Node
- Export Mobile flag
- Physics ApplyTorque node
- Targa Alpha support (internal conversion)
- Trait props used in favor of parameters
- Trait panel has icons!
- Support for multiple material parameters
- Read file/Read JSON and Write file/Write JSON nodes
- Blend and Discard for forward solid
- Billboard for forward solid
- Tilesheet for forward solid
- Renderpath search and renderpath popup
- Shadow Cubemap bias
- Props can now be set
- Clustered rendering (Deferred and Forward)
- Ray Cast has hit normal socket
- Faster shadow sampling
- Voxel Ambient Occlusion support for HLSL
- Threaded path for shader compilation
- Hashlink (HL/C) support
- HTML WebGL2 Support
- Custom target support?
- General speed overhaul
- Physics Rigid Body On Contact node
- More Shadow Cubemap props exposed
- Improved light sampling
- Fast Exporter
- Fixed logic node search
- New B.28 caching
- Krom patching instead of builds with viewport
- Project Panels
- Individual light shadow toggle
- B.28 collections support (Replaces groups)
- Armory terrain support
- Terrain physics trait
- Exporter takes gravity field weights into account (Custom gravity direction)
- Improved movie handling (Still only HTML5)
- SSR for forward path
- Voxel AO Shadows
- Attenuation for area lights
- Haxe compilation server (On by default now!)
- Volumetric clustered support
- Exposed VoxelAO Shadow Cone aperture
- Resize for HTML5 target
- Canvas Get and Set slider nodes!
- Exposed vignette strength!
- Expanded material blending panel
- In Array node
- Dynamic Voxel Allocation
- Translate node has local axis option!
- Material existance check
- Raytracing DirectX Compiler
- Histogram/Autoexposure/EyeAdaption support
- Cloud radiance
- Reworked water data
- Water refraction
- Reworked world settings (Better water and clouds!)
- Deprecated node replacement on project clean
- RotateObjectAroundAxis node
- Khafile parameter is now exposed
- Automatic radiance generator scaling
- Single-Data-File exporter option
- Updated film transparent support
- Armory uses Color management exposure rather than film exposure
- Blend and Alpha testing for overlays
- Micro Shadowing support
- Updated math node

*The above list is incomplete, and only some a described/illustrated. Feel free to comment about missing features on this list, provide examples/images of the features below*
