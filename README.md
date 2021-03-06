DLight is a texture pack for Minecraft Bedrock.
It does not yet have all textures.

I'm a Linux user, and primarily intend to work on this on my workstation using GIMP
and Python.

Python is used for:
* Bumping the version string
* Refreshing the UUID
* Verifying that all textures mentioned in the json are present
* (Re)Generating some textures, like glass and lava
* And that all texture files are in the correct format, size, and so on

## Making it installable
Remember that a .mcpack file, which minecraft will install when you double click on it, is just a zipfile with the manifest.json in the toplevel. So to make this thing installable, make your zipfile that way and just double-clock on it. The "mcpack" script handles this for you.

## Uses: Mixing it up
For the foreseeable future you will likely want to mix this texture pack with one or more other texture packs; it will be a long time before I have coverage of all textures, if that ever even happens. You might instead just use this to understand how texture packs work and what kinds of scripting you might do around them. I use nVidia's sample pack.

## See also:
* [Showcase: Stone](showcase_stone.md)
* [Showcase: Non-Stone](showcase_nonstone.md)
* [Showcase: Items](showcase_item.md)
* [Technical Notes](NOTES.md)

## On Java
I have never had an install of Minecraft Java so I have no idea if this will work on that platform.

## Useful references
* The current default texture pack - https://www.minecraft.net/en-us/addons (link is just above INSTALLATION INSTRUCTIONS)
* Another texture pack on github - https://github.com/ZtechNetwork/MCBVanillaResourcePack
* NVIDIA's docs and "pixelart" PBR texture pack - https://www.nvidia.com/en-us/geforce/guides/minecraft-rtx-texturing-guide/
* Bedrock wiki - https://wiki.bedrock.dev/concepts

## PBR production
This summarises the Minecraft RTX texturing guide (which you should skim) and describes a process

A texture (example: diorite) is composed of:
* A JSON file - diorite.texture\_set.json
* Primary texture: diorite.png - Obvious how this works. Alpha channel is opacity, if relevant
* MER: diorite\_mer.png - R:Metallicity, G:emissivity, and B:roughness. To edit this in GIMP, use Colours:Components:Decompose, edit the layers, and then use Colors:Components:Recompose to rejoin them. This file does not need an alpha channel and can be RGB.
* Normals: diorite\_normal.png - Optional, gives illusion of depth. Let's not mess with this for now. There are some GIMP filters that might be usable whenever we might decide this is important.

For MER:
* Red/Metallicity: nVidia recommends this be effectively boolean
* Green/Emissivity: This can sensibly be scalar, from 0 (unlit) to 1 (bright)
* Blue/Roughness: This can sensibly be scalar, from 0 (smooth) to 1 (rough)

