# Dirt and dirt-based textures
## Dirt
[!Dirt](dlight/textures/blocks/dirt.png?raw=true)

Should give a feel of a lot of different stuff, slowly blending, and roughly grouped into clumps. Varying shades of browns, oranges, pale yellows, and the like. I applied a filter after finishing the texture that helped make it gritty, and saved a prefiltered version to a "junk drawer" directory in the git repo.

## Dirt
[!Mycelium Side](dlight/textures/blocks/mycelium_side.png?raw=true)
[!Mycelium Top](dlight/textures/blocks/mycelium_top.png?raw=true)

From the side, based on dirt with a "blueberry joghurt" topping, composed of many shades of blue/purples, speckly in places. We add some speckles in the dirt layer too, to resemble the roots digging into the soil. The top texture is made from scratch with the same colours and design motifs, largely.


# Glasses
## Plain Glass (full pane)
![Glass](dlight/textures/blocks/glass_mer.png?raw=true)
(the glass texture is a TGA file and browsers cannot render that, so this is the PBR image instead. Ignore the colours)

Entirely transparent apart from the edges, which have 3 shades of grey on the boundaries representing the frame. Has 2 layers of small stylings in each corner that echo the corner with glass between, followed by a dot. In the upper-left styling there is a mistake (that turned out well) of a dot to the right of and between the stylings. This was going to be another suspended line echoing the top border; that idea was scrapped but the first dot was accidentally left in. The irregularity looks cool so it will not be touched out, and if this is ever redesigned it may be left in.

## Other full panes of glass
Will likely be built from plain glass and just slightly tinted. Likely by a software script. This is not yet implemented.

# Sands
## Standard Sand
![Sand](dlight/textures/blocks/sand.png?raw=true)

Cloudy yellow-brown based on real photographs of sand. Darker portions look a bit wet. Has dark speckles in it. Designed, like gravel, to look like it'd definitely fall down/apart if unsupported.

## Red Sand
![Red Sand](dlight/textures/blocks/red_sand.png?raw=true)

Based on standard sand, with a hue shift towards red.

# Soul Surfaces 
## Soul Sand
![Soul Sand](dlight/textures/blocks/soul_sand.png?raw=true)

Deep red background with brighter faces at varying orientations embedded. Darker swirls around and between those faces. A small number of brown highlights. The face features themselves should emit a small amount of light.

## Soul Soil
![Soul Soil](dlight/textures/blocks/soul_soil.png?raw=true)

Based off soul sand, with the faces removed and replaced by flatter, cracked areas. Red hue is significantly diminished. As face features are gone, so is the light emission.

# Glazed Terracottas
## White Glazed Terracotta
![White Glazed Terracotta](dlight/textures/blocks/glazed_terracotta_white.png?raw=true)

Based on the standard texture very strongly for the blue portions (but higher res and more curve-y), less so for the orange sections which take somewhat different shapes and in some places have orange overtones. Hard to describe further because of the complexity of the design. Maintains the diagonal symmetry of the original.

## Gray Glazed Terracotta
![Gray Glazed Terracotta](dlight/textures/blocks/glazed_terracotta_gray.png?raw=true)

Based on the broad shapes from the original, but with a lot of embellishments and differences.

## Green Glazed Terracotta
![Green Glazed Terracotta](dlight/textures/blocks/glazed_terracotta_green.png?raw=true)

Based loosely on the original texture; many embellishments and differences. Maintains both the edge and diagonal symmetry of the original.

## Orange Glazed Terracotta
![Orange Glazed Terracotta](dlight/textures/blocks/glazed_terracotta_orange.png?raw=true)

Based loosely on the original texture; many embellishments and differences. Maintains symmetries of the original.

Variant of netherrack with pale purple protrusions of mostly rounded shapes placed reasonably randomly in the block. These glow and look largely all right. Might have been better off making them white rather than pale purple; may yet make that revision.

# Trees
## Birch
![Birch Log](dlight/textures/blocks/log_birch.png?raw=true)

Ranges in colour from a light grey to pale yellow. Darker stripes going across, with some knots.

# Lava
## Still lava
![Still lava](dlight/textures/blocks/lava_still.png?raw=true)

For this, I used GIMP's lava script-fu generator, removing the border that tool makes and then applying some simple animation filters on it to generate variants. I cut'n'paste them back together into the expected format. A fair bit of work, but more process than art.

## Flowing lava

![Still lava](junk_drawer/lava10_base.png?raw=true)

For this, I again used GIMP's lava script-fu generator, with a different setting, removed the border, applied a "seamless tile" filter (probably better than what I used for still lava), and saved it to a base texture that is displayed above. I then used a script I wrote called makeshiftset to generate rotated versions of that to perform the appropriate shifts to make the texture seem to flow. This is still pretty experimental, but it hopefully will do the job.

# Ice
## Regular ice
![Ice](dlight/textures/blocks/ice.png?raw=true)

I took inspiration from the default ice texture, and did diagonal streaks of various light blue shades. I went with the same transparency scheme, more-or-less, as nVidia's ice texture but appropriate to our texture.

## Packed ice
![Packed Ice](dlight/textures/blocks/ice_packed.png?raw=true)

Based on ice, but with no transparency, and with higher-intensity blue highlights added. Using the same simple MER that nvidia uses.

## Blue ice
![Blue Ice](dlight/textures/blocks/blue_ice.png?raw=true)

Based on packed ice, but with most patterns softened by brushes of an intense blue. To make things interesting, added diagonal stripes of an even deeper blue in small lines.

# Misc
## Glowstone
![Glowstone](dlight/textures/blocks/glowstone.png?raw=true)

Primarily yellow with 4 sine waves going across, each "leaning" forward or backwards. Some colour variations to keep things interesting.

## Slime
![Slime](dlight/textures/blocks/slime_mer.png?raw=true)
(the slime texture is a TGA, which lacks browser support. This is instead the MER, so ignore the colour)

Light green with blotches. Darker green square in the middle. Mostly smooth with some cracks in the mer.

## Web
![Web](dlight/textures/blocks/web_mer.png?raw=true)
(the web texture is a TGA file and browsers cannot render that, so this is the PBR image instead. Ignore the colours)

A fairly random/realistic looking spider web. Not particularly symmetric like the standard texture.

