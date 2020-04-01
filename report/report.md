# Survey of Free Software Within the Gaming Industry

# Table Of Contents

1. [Introduction](#1-introduction)
2. [Findings](#2-findings)
	1. [General Findings](#1-general-findings)
		1. [Game Engines](#1-game-engines)
		2. [UI Libraries](#2-ui-libraries)
		3. [Sound Libraries](#3-sound-libraries)
		4. [Physics Engines](#4-physics-engines)
		5. [Multimedia and General Libraries](#5-multimedia-and-general-libraries)
		6. [External Development Tools](#6-external-development-tools)
		7. [Assets](#7-assets)
	2. [Free and Open Source Software Communities](#2-free-and-open-source-software-communities)
3. [Remarks](#3-remarks)
	1. [Licensing Considerations and Caveats](#1-licensing-considerations-and-caveats)
	2. [Areas Not Covered](#2-areas-not-covered)
4. [Conclusion](#4-conclusion)
5. [References](#5-references)

# 1. Introduction
As the gaming market grows and games continue to become more complex, there has been an interest in finding libraries and tools that have already been made, instead of developing them from the ground up. However, one concern often found in licensing software is that many licenses have restrictions for use on them. For some software, a license may not allow you to modify the library or tool without needing an additional license, or may require you to obtain multiple licenses of the software for each system you are using for development. Free and Open Source Software serves to address these restrictions by providing licenses that allow developers more freedom in using and modification of the software.

Free and Open Source Software is more than just software that has accessible source code. The definition of "Free and Open Source" varies, and in reality "Free software" and "Open Source software" are two different terms with differing communities, histories, and goals. For this article, we will be using the term "Free Software" and focus on how free software is defined according to the [Free Software Foundation](https://www.fsf.org/), as well as using the term "freely licensed" to describe something that follows by these guidelines. The Free Software Foundation's definition of free software consists of four basic rights that free software must guarantee:

1. The freedom to run the program
2. The freedom to access and modify the source code in any way
3. The freedom to redistribute copies of the program
4. The freedom to distribute copies of the software, whether containing your own changes or not

When developors provide these freedoms by providing a free software license, the software can be modified and used for other projects, allowing that software to fill in gaps in other programs, or to avoid writing certain logic again when the libraries already exist. Free software can also help to simplify certain areas of the game development process, especially when a developer lacks experience within a certain field. By removing the need to develop these extra areas, developers can focus on the aspects of the game, game engine, or tools they desire. An independent game developer, for example, can focus on improving the gameplay of their project, while a AAA who need an audio engine to replace their current one can have their developers integrate one that already exists.

This paper provides a look into the field of free software and tools related to video game development. This paper will look into what areas of the game market are flourishing with free software and which areas are lacking. The scope of this paper does not cover how to setup libraries or what resources are best for a project, nor is this a guide about what libraries to use.

Licensing and the implications of certain licenses are a complex field, and beyond the scope of this paper. There are, however, several resources containing information about licenses, including the Open Source Initiative's [Licenses & Standards](https://opensource.org/licenses) page, the Free Software Foundation's [Various Licenses and Comments about Them](http://www.gnu.org/licenses/license-list.en.html), and Karl Fogel's [Producing Open Source Software](https://producingoss.com/).

# 2. Findings

## 1. General Findings
Overall, free software in the game is very much alive and well. There are several tools, software libraries, and assets that are open sourced and are used by many different game developers, and from small personal projects such as [Archipelago](https://store.steampowered.com/app/513720/Archipelago/), to large scale AAA games and engines such, such as [Rainbow 6 Siege](https://www.ubisoft.com/en-us/game/rainbow-six/siege). For ease of reference, the following categories are defined and discussed:

1. Game Engines
2. UI Libraries
3. Sound Libraries
4. Physics Engines
5. Multimedia and General Libraries
6. External Development Tools
7. Assets

### 1. Game Engines
For some developers, creating and developing all aspects of the a game from scratch is unnecessary. A lot of developers may not have the time, motivation, knowledge, or even interest in developing each aspect of a game from scratch. Game engines are tools that provide a way for game developers to focus easily on developing their game rather than their technology, usually by packaging the fundamental parts of a game together, such as physics and a graphics pipeline. Some of the freely licensed game engines include:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [Godot](https://godotengine.org/) | MIT | 2D and 3D game engine using a custom scripting language and C# support |
| [Torque 3D](http://www.garagegames.com/products/torque-3d) | MIT | 3D game engine using a custom scripting language for development |
| [PlayCanvas](https://playcanvas.com/) | MIT | 3D web based game engine using JavaScript for development |
| [Irrlicht](http://irrlicht.sourceforge.net/) | Zlib | 3D game engine using C++ for development |
| [MonoGame](http://www.monogame.net/) |  MS-PL | 2D and 3D game engine using C# for development |

Each of these engine targets different fields and game types, but they all provide a powerful framework to develop games on. Some examples of these game engine include:
[Octodad: Dadliest Catch](https://store.steampowered.com/app/224480/Octodad_Dadliest_Catch/) a physics based adventure / puzzle game developed on the Irrlicht engine. Octodad: Dadliest Catch was successful as an indie game, reaching almost [500000 in sales in 2015](https://www.polygon.com/2015/2/2/7962611/octodad-sales)

[Frozen Synapse](http://www.frozensynapse.com/) and [Fronzen Synapse 2](https://www.frozensynapse2.com/) both use the Torque 3D. Frozen Synapse and it's sequal are turn-based strategy games.

[Celeste](http://www.celestegame.com/), a 2D platformer developed using MonoGame. Celeste had [sold over 500000 copies by the end of 2018](https://www.gamasutra.com/view/news/333554/Celeste_has_sold_over_500000_copies_since_January.php)

[Battle for Wesnoth](https://github.com/wesnoth/haldric) is being ported to Godot. Battle for Wesnoth is a free and open source turn-based strategy game that was released in 2005, and has been consistantly updated since then.

### 2. UI Libraries
A games user interface, or UI, helps determine how the user interacts with the game and world, and is usually one of the most important parts of a game. Because of this, there exists a healthy number of UI libraries that streamline the process of creating UI elements. Complexity and power of UI libraries tend to vary, from a simple interface with a game engine such as Nuklear, to complex libraries with many different parts such as Qt5. Some free licensed libraries include:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [NanoGUI](https://github.com/mitsuba-renderer/nanogui) | BSD-3-Clause Modified | C++ UI library that is compatible with several graphics APIs |
| [Qt5](https://www.qt.io/) | LGPL-3.0-only, GLP-3.0-only, or GPL-2.0-only | C++ windowing and GUI library |
| [Nuklear](https://github.com/Immediate-Mode-UI/Nuklear) | MIT or Unlicense | Lightweight graphics API that can be accelerated with graphics APIs |
| [ImGUI](https://github.com/ocornut/imgui) | MIT | Immediate mode C++ UI library |

Similar to the game engines, each of these GUI libraries has different projects associated with them. For example:

ImGUI has been used by Ubisoft for creating debugging tools for their games and actually [sponsored ImGUI](https://montreal.ubisoft.com/en/ubisoft-sponsors-user-interface-library-for-c-dear-imgui/). They discuss its use in 2016 by the Assissins Creed team and its later adoption by Rainbow 6: Siege.

[C-Dogs SDL](https://cxong.github.io/cdogs-sdl/), a freely licensed port of the game C-Dogs, uses Nuklear for it's UI. C-Dogs is a 2D top-down shoot'em up originally released between 1997 and 2001, and later open sourced, allowing a group of developers to develop an SDL port based on the newly released source code.

[OpenClonk](https://www.openclonk.org/), a continuation of the Clonk series, uses Qt5. OpenClonk is a multiplayer action game that just recently released version 1.0.0.

### 3. Sound Libraries
Sound is often one of the most important and iconic parts of any game, and helps tie in game events with certain feedback. Within the free software community, there are several available options for sound libraries ranging from low level APIs to high level audio abstractions. Some well known libraries are:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [libnyquist](https://github.com/ddiakopoulos/libnyquist) | BSD-2-Clause | C++ library for decoding audio files |
| [OALWrapper](https://github.com/FrictionalGames/OALWrapper) | Zlib | Wrapper for OpenAL written in C++ |
| [OpenAL Soft](https://kcat.strangesoft.net/openal.html) | LGPL-2.0-only w/ some BSD-3-Clause | Software implementation of the OpenAL specification|
| [Port Audio](http://www.portaudio.com/) | MIT | C++ library for playing and recording sounds |
| [LabSound](https://github.com/LabSound/LabSound) | BSD-2-Clause | Graph based audio engine in C++ |

Well games and software based on these libraries include:

The [Penumbra series](www.penumbragame.com/), which uses OALWrapper. Penumbra was the first series of horror games by Frictional Games, and OALWrapper, along with the game engine used in the series, were developed and released by Frictional Games under a free software license.

[Master of Orion III](https://store.steampowered.com/app/410990/Master_of_Orion_3/) uses the Port Audio library. Master of Orion III is a turn-based strategy game originally released in 2003.

[0 A.D.](https://play0ad.com/), a real-time strategy game, uses OpenAL Soft for it's audio. 0 A.D. is licensed under a free software license as well, and all the assets of the game are licensed under the creative commons license.

[Audacity](https://www.audacityteam.org/) uses libnyquist and Port Audio in it. Audacity is a freely licensed audio editing tool.

These sound libraries also provide a good example of building upon open source software, as several of these libraries build upon others. For example, OALWrapper uses OpenAL Soft as a back end, and LabSound builds on top of libnyquist. Many free audio libraries are available to use, while also providing examples for the use of other free software projects in another project.

### 4. Physics Engines
Most games usually need some sort of physics system for their gameplay. Because physics is both a fundamental part of many games, and since physics can quickly become complex, there are several powerful free software physics engines for both 2D and 3D physics that can be integrated into any game. Some of the most notable of these engines are:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [Bullet Physics](https://pybullet.org/wordpress/) | Zlib | Accelerated 3D physics engine |
| [Newton Dynamics](http://www.newtondynamics.com/forum/newton.php) | Zlib | 3D physics engine for C++ |
| [PhysX](https://www.geforce.com/hardware/technology/physx) | BSD-3-Clause | 3D physics library with hardware acceleration for NVIDIA GPU's |
| [Box2D](https://box2d.org/) | MIT | 2D physics engine for C++ |
| [Open Dynamics Engine](http://ode.org/) | LGPL-2.1-only or BSD-3-Clause | 3D physics engine for C++ |

Each of these have use in several different titles and game engines including:

The previously discussed [Godot](https://godotengine.org/) uses two physics engines: Box2D and Bullet Physics. Since godot has support for both 2D and 3D games, the engine needs to support physics in 2D and 3D.

Frictional Games uses Newton Dynamics in their game engines. This includes the previously mentioned [Penumbra series](http://www.penumbragame.com), as well as the [Amnesia series](https://www.amnesiagame.com/#main) and the game [SOMA](http://www.somagame.com/).

The previously discussed [Torque 3D game engine](https://torque3d.org/), as well as Epic Game's [Unreal Engine](https://www.unrealengine.com/en-US/) and Unity Technologies' [Unity game engine](https://unity.com/) all use NVIDIAs PhysX.

[Panda3D](https://www.panda3d.org/) uses Open Dynamics Engine for its 3D physics. Panda3D is a freely licensed 3D game engine.

An important note is that NVIDIA's PhysX was just recently open sourced, but the freely licensed version is only availble for PC and mobile platforms. It's also interesting to note the large use of several of these physics engines, compared to the smaller use of some of the other libraries.

### 5. Multimedia and General Libraries
There are several other game libraries that do not quite fit well into the other categories, as they fall under multiple of them, fall under none of them, or have parts that fall into both the previous categories. These types of libraries are either general multimedia libraries, or libraries with specific uses. Some of these libraries include:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [SFML](https://www.sfml-dev.org/) | Zlib | General multimedia and library for C++ |
| [SDL](https://www.libsdl.org/) | Zlib | Multimedia and windowing library for C / C++ |
| [GLFW](https://www.glfw.org/) | Zlib | C++ windowing library |
| [GLEW](http://glew.sourceforge.net/) | BSD-3-Clause and MIT | General OpenGL utility |
| [Assimp](http://assimp.org/) | BSD-3-Clause Modified | 3D asset loading library for C++|
| [stb](https://github.com/nothings/stb) | MIT or Unlicense | Set of various useful libraries for game development |

Several of these libraries have been used in different games and game engines, for example:

[Open Hexagon](https://vittorioromeo.info/projects.html) uses SFML. OpenHexagon is a freely licensed recreation of the game Super Hexagon feature custom level creation and editing.

Once again [Godot](https://godotengine.org/) makes use of free software libraries: this time stb and assimp.

[OpenClonk](https://www.openclonk.org/), a previously mentioned game, uses GLEW for windowing.

SDL is an incredibly popular library to use in particlar, with uses ranging from the aforementioned [0 A.D.](https://play0ad.com/) and [Penumbra series](http://www.penumbragame.com), to [Team Fortress 2](http://www.teamfortress.com/) and [FTL: Faster than light](https://subsetgames.com/ftl.html).

Several of these libraries are very popular within the independent game development community, and many can also be seen in the AAA industry as well. These libraries are generally useful for several different areas of game development, which is the main reason why they are seen in several different areas of the gaming industry.

### 6. External Development Tools
There are many different tools for developing and creating content for games. Several of the tools listed here are for content creation, but there are many different tools for development as well. For content creation, available tools include:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [Blender](https://www.blender.org/) | GPL-2.0-or-later | 3D subdivision modeling tool |
| [Krita](https://krita.org/en/) | GPL-2.0-only | 2D raster graphics painting tool and editor |
| [GIMP](https://www.gimp.org/) | GPL-3.0-or-later | 2D raster graphics editor and manipulator
| [Inkscape](https://inkscape.org/) | GPL-2.0-only | 2D vector graphics editor |
| [LMMS](http://lmms.io/) | GPL-2.0-or-later | Digital audio workstation |
| [Ardour](http://ardour.org/) | GPL-2.0-only | Digital audio workstation |
| [Audacity](https://www.audacityteam.org/) | GPL-2.0-or-later | Audio editing tool |

For development, several IDEs include:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [KDevelop](https://www.kdevelop.org) | GPL-2.0-only | IDE for C/C++, QML / JavaScript, Python, and PHP |
| [Qt Creator](https://www.qt.io/development-tools) | GPL-3.0-only | IDE for C/C++, QML / JavaScript, and Qt development |
| [Mono Develop](https://www.monodevelop.com/) | LGPL-2.0-only w/ MIT portions | IDE for C/C++, CIL, D, Java, JavaScript and more |
| [Visual Studio Code](https://code.visualstudio.com/) | MIT for source code, binaries are proprietary | Code editor with support for several programming languages and plugins |

Many of these tools are well known or gaining popularity, and several are available on different platforms, including steam and the windows store.

### 7. Assets
For some developers, it may be useful to find assets for use that follow along the same guidelines as free software. Whether they are needed for testing, or if they will be used in the final product, assets are always important. There are plenty of sites that have freely licensed assets to use, and some with licensing that is similar, but not quite free, as they don't follow the definitions of free software. Regardless, a list of sites available include:

| Name | License(s) | Description |
| ---- | ------- | ----------- |
| [Open Game Art](https://opengameart.org/) | Various, including CC and GPL varieties | General open source game art assets |
| [Open Pixel Project](http://www.openpixelproject.com/) | CC0-1.0 | Art assets with a focus on 2D pixel art |
| [CC0 Textures](https://cc0textures.com/) | CC0-1.0 |  textures and materials |
| [Free PBR](https://freepbr.com/) | Non-free | free to use PBR textures, but not open source (doesn't allow redistribution) |
| [Kenney Game Assets](https://kenney.nl/assets) | CC0-1.0 | General game assets |
| [Game-icons.net](https://game-icons.net/) | CC-BY-3.0 | UI assets |
| [Incompetech](https://incompetech.com/music/royalty-free/) | CC-BY-3.0 or proprietary | Music that is also available to purchase if attribution is not wanted / possible |
| [SoundBible](http://soundbible.com/tags-game.html) | Varioud CC, public domain, and some non-free | Sound effects that are mostly CC-BY-3.0 |

Overall, there are plenty of sites with open source game assets to use, and finding free assets is an easy task. Several of these sites may contain assets that are recognizable from other games, and several have been used in non-game projects as well.

## 2. Free and Open Source Software Communities
As free software for gaming grows, the communities following, developing and participating in free software continue to grow as well. Currently, there are plenty of open source game development and gaming communities that exists. Most of these communities exist on several different platforms, including online forums, IRC channels, and social media. There are several communities focused on specific games, usually involving their own forums and IRC channels, and there is a growing community around specific game engines. Godot, for example, has gained a significant following in the open source community using many channels of communication, including IRC, a subreddit, a steam page and a facebook page, and has started to gain the interest of many game developers. Similarly, the game [Battle for Wesnoth](https://wesnoth.org/) makes use of steam, facebook, and reddit, while also running a custom forum for its community.

# 3. Remarks
While the world of free software within the game industry is vast, there are still important things to note. The first important notes are in regards to licensing. The second set are in regards to the limitations of this paper and the areas not covered by it.

## 1. Licensing Considerations and Caveats
Some open source software and assets have dual licensing. This means that there's usually a choice between different types of licenses for the source, and is usually meant to add an easier way to use the library commercially. Some libraries and assets have different parts under different licenses as well. An excellent example of this is Qt. Qt packages are available under different licenses depending on the package, as well as under the option of a proprietary license. This may be important to keep in mind depending on if you plan on contributing or extending the library you are using, as certain packages may force you to release your code under the same license, while others may not.

Finally, OpenAL and OpenGL are both technically standards with several different implementations. While some implementations, such as OpenAL Soft, are free software, not all implementations of these libraries are, and many times these libraries will be included automatically with an operating system or with drivers.

## 2. Areas Not Covered
As there are an endless amount of free software libraries and freely licensed assets, this paper cannot cover all of them. Some areas with free software that are not discussed within this list include:

* Scripting libraries
* Networking libraries
* Artificial Intelligence libraries
* Threading libraries
* Memory Management libraries

Each of these areas have free software libraries available, and readers are encouraged to seek out and find open source alternatives to what they may be looking for. Some sites that may be of use may include:

* Wikipedia's [List of Open Source Video Games](https://en.wikipedia.org/wiki/List_of_open-source_video_games), which itself provides links to other free software topics and lists.
* [Open source, experimental, and tiny tools roundup](http://everest-pipkin.com/teaching/tools.html), a game centric list of various tools and libraries, some of which are free software.

Finally, for resources on licensing, sites to look at include:

* [Various Licenses and Comments about Them](http://www.gnu.org/licenses/license-list.en.html) from the Free Software Foundation
* [Various Licenses and Comments about Them](http://www.gnu.org/licenses/license-list.en.html) from the Open Source Initiative
* [Producing Open Source Software](https://producingoss.com/) by Karl Fogel
* [Choose a License](https://choosealicense.com/) from GitHub

# 4. Conclusion
Overall, there is quite a health list of free software available within the gaming industry. There are several areas of game development that have a healthy selection of libraries and tools available to use for game development, as well as a large number of available tools and resources. There are some areas of the game development field that are more lacking in free software or are more concentrated on a few libraries / software, but as the open source community grows, it makes sense to also expect growth in these areas too. Free software and the open source community are gaining a strong presence within gaming, with a growing amount of free software and tools being used by more game developers and companies.

# 5. References
“Ardour.” Ardour, http://ardour.org/.

“Audacity.” Audacity, https://www.audacityteam.org/.

“Blender.” Blender, https://www.blender.org/.

“Box2D.” Box2D, https://box2d.org/.

“Bullet Physics.” Bullet Real-Time Physics Simulation, https://pybullet.org/wordpress/.

“CC0 Textures.” CC0 Textures, https://cc0textures.com/.

“Choose an Open Source License.” Choose a License, https://choosealicense.com/.

“Free PBR.” Free PBR, https://freepbr.com/.

“Game Sounds.” Sound Bible, http://soundbible.com/tags-game.html.

“Game-Icons.Net.” Game-Icons.Net, https://game-icons.net/.

“GIMP.” GIMP, https://www.gimp.org/.

“GLFW.” GLFW, https://www.glfw.org/.

“Godot Engine.” Godot, https://godotengine.org/.

“ImGUI.” GitHub, https://github.com/ocornut/imgui.

“Incompetech.” Incompetech, https://incompetech.com/music/royalty-free/.

“Inkscape.” Inkscape, https://inkscape.org/.

“Irrlicht.” Irrlicht, http://irrlicht.sourceforge.net/.

“KDevelop.” KDevelop, https://www.kdevelop.org.

“Kenney.” Kenney, https://kenney.nl/assets.

“Krita.” Krita, https://krita.org/en/.

Kuchera, Ben. “Octodad Shares the Reality of an Indie Hit: $4.9M in Revenue for 2.7 Years of Work.” Polygon, https://www.polygon.com/2015/2/2/7962611/octodad-sales.

Kurr, Chris. “Celeste Has Sold over 500,000 Copies since January.” Gamasutra, https://www.gamasutra.com/view/news/333554/Celeste_has_sold_over_500000_copies_since_January.php.

“LabSound.” GitHub, https://github.com/LabSound/LabSound.

“Libnyquist.” GitHub, https://github.com/ddiakopoulos/libnyquist.

“LMMS.” LMMS, http://lmms.io/.

“MonoDevelop.” MonoDevelop, https://www.monodevelop.com/.

“MonoGame.” MonoGame, http://www.monogame.net/.

“NanoGUI.” GitHub, https://github.com/mitsuba-renderer/nanogui.

“Newton Dynamics.” Newton Dynamics, http://www.newtondynamics.com/forum/newton.php.

“Nuklear.” GitHub, https://github.com/Immediate-Mode-UI/Nuklear.

“NVIDIA PhysX.” NVIDIA, https://www.geforce.com/hardware/technology/physx.

“OALWrapper.” OALWrapper, http://frictionalgames.github.io/OALWrapper/.

“Open Dynamics Engine.” Open Dynamics Engine, http://ode.org/.

“OpenAL Soft.” OpenAL Soft, https://kcat.strangesoft.net/openal.html.

“OpenGameArt.Org.” OpenGameArt.Org, https://opengameart.org/.

“OPP.” OPP, http://www.openpixelproject.com/.

“PlayCanvas.” PlayCanvas, https://playcanvas.com/.

“PortAudio.” Port Audio, http://www.portaudio.com/.

“Qt.” Qt, https://www.qt.io/.

“Qt Creator IDE.” Qt, https://www.qt.io/development-tools.

“SDL.” SDL, https://www.libsdl.org/.

“Simple and Fast Multimedia Library.” SFML, https://www.sfml-dev.org/.

“Stb.” GitHub, https://github.com/nothings/stb.

“The Open-Asset-Importer-Lib.” The Open-Asset-Importer-Lib, http://assimp.org/.

“The OpenGL Extension Wrangler Library.” GLEW, http://glew.sourceforge.net/.

“Torque 3D.” GarageGames, http://www.garagegames.com/products/torque-3d.

“Various Licenses and Comments about Them.” GNU Operating System, http://www.gnu.org/licenses/license-list.en.html.

“Visual Studio Code.” Visual Studio Code, https://code.visualstudio.com/.