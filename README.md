# LAMA - Landscape AutoMaterial with manual pAinting 

I've created simple automaterial for landscape painting based on slope and height and which allows for manual painting as well. I've tried to make it easy to extend and modify in the future so I've divided the material between multiple material functions: set of functions for layers, set of functions for auto-paiting layers and a set of helper function that make it happen.

# Current features
- manual & automatic painting 
- 4 textures for manual painting and 4 textures for automatic painting (extensible to more)
- Automatic painting based on height and slope
- UV Mixing (anti-tilling)
- Nosie-based anti-tiling (detail)
- tesselation/displacement map
- easy to extend ;-)

Feel free to suggest additional features, I'll try to add them.

# Some current LAMA limitations:
- Default textures used with LAMA are not ideal. For small size of repo I used only 1k textures and packed displacement maps myself. Displacement maps for them are not perfect (I might have messed up something while packing them up. 
- Only 1 automatic layer is using slope blending.
- Auto-textures are not reused for manual painting. It would be trival to do in one big graph, but I'm thinking of more elegant way to do it . Please share if you have idea how to accomplish it and I'll add it to LAMA.
- The transition between auto-layers based on height is gradual, but boring. I am thinking on a way to add some kind of noise that would simulate e.g., snow melting with different speed in differnt places (not in a uniform way like now). If you have some ideas how to add it - let me know.

# Tutorials

I foresee 3 basic use cases for LAMA.
1. Taking it and using it straight away for your projects. See: https://forums.unrealengine.com/community/community-content-tools-and-tutorials/1594589-free-landscape-automaterial-with-manual-painting?p=1594930#post1594930
2. Taking it and adapting it to your needs. (description: TBD)
3. Learning from it to use only the knowledge in your projects. (description: TBD)

# Copyright notes

This project is released under MIT licence, but please note that I've learned most of it from the following sources:
- Epic's Getting Started with Landscapes (https://www.youtube.com/watch?v=gMKjIZMPJ0Q), esp. MF_AntiTillingNoise is based on what was shown there and I claim no copyright on it.
- [Unreal Engine 4] Automated Terrain Texturing blog post inspired me how to do slope and height blending http://oliverm-h.blogspot.com/2014/08/unreal-engine-4-automated-terrain.html 
- RATSGAME youtube tutorials showed me how to join both manual and automatic paiting of terrain https://www.youtube.com/playlist?list=PL2G_ecHWhZBmEQih1qfe4yIzY49tKxST6

**Textures are CC0** from https://texturehaven.com/. Really excellent stuff, go there for high resolution ones. And if you are able to support Rob - do so :)

FakeWater is based on excelent tutorial by Andrew Hurley https://wiki.unrealengine.com/Water_Shader_Tutorial (largely simplified it, it is just a place holder :) ).
