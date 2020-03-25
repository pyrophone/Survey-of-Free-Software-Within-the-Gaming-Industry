# Survey of Free Software Within the Gaming Industry

# Table Of Contents

1. Introduction
2. Findings
	1. General Findings
		1. Game Engines
		2. UI Libraries
		3. Sound Libraries
		4. Physics Engines
		5. Multimedia and General Libraries
		6. External Development Tools
		7. Assets
	2. Free and Open Source Software Communities
3. Remarks
	1. Licensing Considerations and Caveats
	2. Areas Not Covered
4. Conclusion
5. References

# 1. Introduction
As the game development market grows, there are more opportunities for new developers to enter and create their own games. With these new developers, there is a greater need for finding libraries and tools that can be freely used with no cost or concerns over licensing. This is where the importance of Free and Open Source Software makes its appearance.

Free and Open Source Software is more than just software that has accessible source code. While the definition of "Free and Open Source" varies, in general, there are four rights that free software must guarantee:

1. The freedom to run and use the program for whatever you wish
2. The freedom to access and modify the source code in any way
3. The freedom to redistribute copies of the program
4. The freedom to distribute copies of your changed files

By providing these freedoms, software that is Free and Open Source can be modified and used for other projects, allowing that software to fill in gaps in other programs, or to avoid writing certain logic again when the libraries already exist. Free and Open Source Software can also help to simplify certain areas of the game development process, especially when a developer lacks experience within a certain field.

This paper serves to provide a look into the market of Free and open Source software and tools related to video game development. This paper will look into what areas of the game market are flourishing with free software and which areas are lacking. It is important to note that the scope of this paper does not cover how to setup libraries or what resources are best for a project. It is also important to note that this is not a guide about what libraries to use. All of these topics will be left for the developer to research and decide on their own.

It is also important to note that licensing and the implications of certain licenses are a complex field, and also out of the scope of this paper. There are, however, several resources containing information about licenses, including GitHub's [Choose an open source license](https://choosealicense.com/) and the Free Software Foundation's [Various Licenses and Comments about Them](http://www.gnu.org/licenses/license-list.en.html). It is worth mentioning that most open source projects, simply using the project for development will not require you to license your project under a free and open source license. On the other hand, modifying a project may require you to do so, which is why it is always important to understand a software's license.

# 2. Findings

## 1. General Findings
Overall, Free and Open Source Software in the game is very much alive and well. There are several tools, software libraries, and assets that are open sourced and are used by both independent and professional game developers alike, and from small personal projects to large scale AAA games. For ease of reference, the following categories are defined and discussed:

1. Game Engines
2. UI Libraries
3. Sound Libraries
4. Physics Engines
5. Multimedia and General Libraries
6. External Development Tools
7. Assets

### 1. Game Engines
For some developers, creating and developing all aspects of the a game from scratch is unnecessary, and gets in the way of development time. Game engines provide a way for game developers to easily focus on developing their game rather than their technology. Overall, there are quite a few powerful free and open source game engines available for both 2D and 3D games. Some of the most popular and powerful game engine include:

* [Godot](https://godotengine.org/)
* [Torque 3D](http://www.garagegames.com/products/torque-3d)
* [PlayCanvas](https://playcanvas.com/)
* [Irrlicht](http://irrlicht.sourceforge.net/)
* [MonoGame](http://www.monogame.net/)

Each of these engine targets different fields and game types, but they all provide a powerful framework to develop games on. Each of these engines has also been the foundation of a well known or successful game. From Octodad (Irrlicht engine), to Frozen Synapse (Torque 3D), to Celeste (MonoGame), to a remake of Battle of Wesnoth (Godot), free and open source game engines are being actively utilized to create many different types of games, including titles that are commercially successful or well known in general.

### 2. UI Libraries
One of the most important aspects of a game is the user interface, or UI. UI's determine how the user interacts with the game and world, and are almost always important for gameplay. Because of this, there exists a healthy number of UI libraries that streamline the process of creating UI elements. Complexity and power of UI libraries tend to vary, from simple interface with a game engine, to complex libraries with many different parts. Some well know libraries include:

* [NanoGUI](https://github.com/mitsuba-renderer/nanogui)
* [Qt5](https://www.qt.io/)
* [Nuklear](https://github.com/Immediate-Mode-UI/Nuklear)
* [ImGUI](https://github.com/ocornut/imgui)

Similar to the game engines, each of these GUI libraries has several well know projects associated with them. For example, ImGUI has been used by Ubisoft for creating debugging tools for their games, Battlefield 3 and C-Dogs SDL both use Nuklear, and OpenClonk uses Qt5. As you can see, several of these libraries have been used in projects ranging from small free and open source games, all the way to large AAA games.

### 3. Sound Libraries
Sound is an often forgotten part of the gaming experience. Despite this, it is often one of the most important and iconic parts of a game. Within the free and open source software community, there are several available options for sound libraries ranging from low level APIs to high level audio abstractions. Some well known libraries are:

* [libnyquist](https://github.com/ddiakopoulos/libnyquist)
* [OALWrapper](https://github.com/FrictionalGames/OALWrapper)
* [OpenAL Soft](https://kcat.strangesoft.net/openal.html)
* [Port Audio](http://www.portaudio.com/)
* [LabSound](https://github.com/LabSound/LabSound)

Well known games and software based on these libraries include the Penumbra series (OALWrapper), Master of Orion III (Port Audio), 0 A.D. (OpenAL Soft), and Audacity (libnyquist, Port Audio). These sound libraries also provide a good example of building upon open source software, as several of these libraries build upon others. For example, OALWrapper uses OpenAL Soft as a back end, and LabSound builds on top of libnyquist. Many free and open source audio libraries are available for different game projects to use, while also acting as good examples of how to use other free and open source projects in another project.

### 4. Physics Engines
Most games usually need some sort of physics system for their gameplay. Because physics is both a fundamental part of many games, and since physics can quickly become complex, there are several powerful free and open source physics engines for both 2D and 3D physics that can be integrated into any game. Some of the most notable of these engines are:

* [Bullet Physics](https://pybullet.org/wordpress/)
* [Newton Dynamics](http://www.newtondynamics.com/forum/newton.php)
* [PhysX](https://www.geforce.com/hardware/technology/physx)
* [Box2D](https://box2d.org/)
* [Open Dynamics Engine](http://ode.org/)

Each of these have use in several different titles and game engines including: Godot (Box2D, Bullet Physics), the Penumbra series (Newton Dynamics), Torque 3D (PhysX), and Panda3D (Open Dynamics Engine). An important note is that NVIDIA's PhysX was just recently open sourced, but only for PC and mobile platforms. It's also interesting to note the large use of several of these physics engines, compared to the smaller use of some of the other libraries.

### 5. Multimedia and General Libraries
There are several other game libraries that do not quite fit well into the other categories, as they fall under multiple of them, fall under none of them, or have parts that fall into both the previous categories. These types of libraries are either general multimedia libraries, or libraries with specific uses. Some of these libraries include:

* [SFML](https://www.sfml-dev.org/), a general multimedia and library
* [SDL](https://www.libsdl.org/) a multimedia and windowing library
* [GLFW](https://www.glfw.org/), a windowing library
* [GLEW](http://glew.sourceforge.net/), a general OpenGL utility
* [Assimp](http://assimp.org/), a mesh loading library
* [stb](https://github.com/nothings/stb), a set of useful libraries for game development

Several of these libraries have been used in different games and game engines, such as: 0 A.D. (SDL), Open Hexagon (SFML), Godot (stb and Assimp), and OpenClonk (GLEW). Several of these libraries are very popular within the independent game development community, and many can also be seen in the AAA industry as well. These libraries are generally useful for several different areas of game development, which is the main reason why they are seen in several different areas of the gaming industry.

### 6. External Development Tools
There are many different tools for developing and creating content for games. Several of the tools listed here are for content creation, but there are many different tools for development as well. For content creation, available tools include:

* [Blender](https://www.blender.org/), for 3D models and assets
* [Krita](https://krita.org/en/) and [GIMP](https://www.gimp.org/) for 2D raster graphics editing
* [Inkscape](https://inkscape.org/) for 2D vector graphics creation
* [LMMS](http://lmms.io/) and [Ardour](http://ardour.org/) for audio asset creation
* [Audacity](https://www.audacityteam.org/) for audio asset editing

For development, several IDEs include:

* [KDevelop](https://www.kdevelop.org)
* [Qt Creator](https://www.qt.io/development-tools)
* [Mono Develop](https://www.monodevelop.com/)
* [Visual Studio Code](https://code.visualstudio.com/)

Many of these tools are well known or gaining popularity, and several are available on different platforms, including steam and the windows store.

### 7. Assets
For some developers, it may be useful to find free and open source assets for use. Whether they are needed for testing, or if they will be used in the final product, assets are always important. There are plenty of sites that have free and open source assets to use, and some with licensing that is similar, but not quite free and open source. Regardless, a list of sites available include:

* [Open Game Art](https://opengameart.org/), general open source game art assets
* [Open Pixel Project](http://www.openpixelproject.com/), game art assets with a focus on 2D pixel art,
* [CC0 Textures](https://cc0textures.com/), Creative Commons PBR textures and materials
* [Free PBR](https://freepbr.com/), free to use PBR textures, but not technically open source
* [Kenney Game Assets](https://kenney.nl/assets), general Creative Commons game assets
* [Game-icons.net](https://game-icons.net/), Creative Commons and public domain UI assets
* [Incompetech](https://incompetech.com/music/royalty-free/), Creative Commons music that are also available under a standard license
* [SoundBible](http://soundbible.com/tags-game.html), various sound effects that are mostly Creative Commons and Public Domain, with some using non-free licenses

Overall, there are plenty of sites with open source game assets to use, and finding free assets is an easy task. Several of these sites may contain assets that are recognizable from other games, and several have been used in non-game projects as well.

## 2. Free and Open Source Software Communities
As free and open source software for gaming grows, the communities following free software continue to grow as well. Currently, there are plenty of open source game development and gaming communities that exists. Most of these communities exist on several different platforms, including online forums, IRC channels, and social media. There are several communities focused on specific games, usually involving their own forums and IRC channels, and there is a growing community around specific game engines. In particular, Godot has gained a significant following in the open source community, and has started to gain the interest of many game developers.

# 3. Remarks
While the world of free and open source software within the game industry is vast, there are still important things to note. The first important notes are in regards to licensing. The second set are in regards to the limitations of this paper and the areas not covered by it.

## 1. Licensing Considerations and Caveats
Some open source software and assets have dual licensing. This means that there's usually a choice between different types of licenses for the source, and is usually meant to add an easier way to use the library commercially. Some libraries and assets are have different parts that are under different licenses as well. An excellent example of this is Qt. Qt packages are available under different licenses depending on the package, as well as under the option of a commercial license. This may be important to keep in mind depending on if you plan on contributing or extending the library you are using, as certain packages may force you to release your code under the same license, while others may not. Finally, it is important to note that OpenAL and OpenGL are both technically standards with several different implementations. While some implementations, such as OpenAL Soft, are free and open source, not all implementations of these libraries are, and many times these libraries will be included automatically with an operating system or with drivers.

## 2. Areas Not Covered
As there are an endless amount of free and open source libraries and assets, this paper cannot cover all of them. Instead, it servers as a general guide to showcase that free and open source alternatives exist, and to show some general areas that they cover. Some areas with free and open source software that are not discussed within this list include:

* Scripting libraries
* Networking libraries
* Artificial Intelligence libraries
* Threading libraries
* Memory Management libraries

Each of these areas have free and open source libraries available, and readers are encouraged to seek out and find open source alternatives to what they may be looking for.
As mentioned previously, it is important to note that this resource is not for learning how to use these any of the libraries, tools, or sites listed, and it is not meant to discuss the advantages and disadvantages of each. This is left for readers to learn about and discover what works best for them.
Finally, this is not a resource on licensing and the history of open source software. Each of those topics are complex, and including them would clutter this resource and take away from its main purpose of acting as an insight into free and open source software for the gaming industry.

# 4. Conclusion
Overall, there is quite a health list of free and open source software available within the gaming industry. There are several areas of game development that have a healthy selection of libraries and tools available to use for game development, as well as a large number of available tools and resources. There are some areas of the game development field that are more lacking in free and open source software or are more concentrated on a few libraries / software, but as the open source community grows, it makes sense to also expect growth in these areas too. Free and open source software and the open source community are gaining a strong presence within gaming, with a growing amount of free and open source software and tools being used by more game developers and companies.

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