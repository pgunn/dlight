This is to document nonintuitive things about making textures, in hopes of helping others who are interested in making textures.

## Versions
It helps to put the version number in the description for a texture pack. My "newversion" script handles this and bumps the UUID too. The Minecraft UI does not have a good display for versions (for now), so do your users a favour and make it visible.

## Transparency
I have heard (but not verified) that it is only valid to use transparency with certain blocks; this makes sense as otherwise people would modify most blocks to be transparent for PVP, and also because Minecraft does certain optimisations with regards to what blocks exist that have not been exposed yet; allowing all blocks to be transparent would ruin such optimisations.

## Emissivity
Don't go overboard with emissivity in MER. The upper bounds of the value scale are ridiculously bright.

## Grass
I believe the reason that grass does not have a colour in its textures is that it displays differently in some biomes, so the textures are leaving room for an interaction between the renderer and biome id to finish the colouration.

## Torches
I haven't figured this one out yet, although I get that a lit torch is a mix of a block texture for the basic shape and a particle effect and those must line up for things to work right. There may be a fixed geometry that torches must have around which the texture must fit.

## Glazed Terracotta
Most glazed terracottas are designed to have fold rather than wrap symmetry in the default texture pack; a few have both. The nVidia texture packs have blank textures for a lot of these (making good textures for these is high-effort and it's not surprising they skipped out and focused on other things.

## Lava
I am operating under the theory that the lava flow texture is a cleverly shifted version of the normal lava texture, designed so that each frame is offset enough that when cycled there will be an impression of motion. At the 32x version of the texture nvidia provides, this shifts by what looks like 1-2 pixels every time, and has 16 frames of animation. Let's assume it shifts by 2 because that would have it cyclic. For our preferred texture size (64), we will need to shift by more assuming we must keep the same number of frames.

## Glass
Colored glass is generated from my standard glass texture by my make\_glass\_variants script. It depends on specifics of that original image, and would need adjustments to work with other images (depending on how different they are, possibly an entirely different approach would be necessary).

## Swords
My initial experimentations with making sword textures (which are not block textures) show me that the item-bar representation is the same image as what's swung in the hand. When in the hand, the upper-left corner is treated as "forward" and the object is given some artificial thickness. An extra JSON file is used to note item textures (unclear if this is mandatory or just to speed imports). The stock texture pack uses indexed colour rather than the standard RGBA colour space; I'm guessing that images that don't do that can't get effects like enchanted swords, but they clearly work. Sharp rather than soft edges around image content is probably desirable.

## Smooth stone
Uses the stone\_slab\_top texture for all faces. Weird legacy stuff going on there.
