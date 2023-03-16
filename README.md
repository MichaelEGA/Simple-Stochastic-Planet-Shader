# Simple-Stochastic-Planet-Shader
A simple procedural planet shader with stochastic texturing

Get it here: https://github.com/michael-evan-allison/Simple-Stochastic-Planet-Shader

Tested In: Unity URP 2022.2.9f1

Version History

17/03/2023 - Initial commit

Planet Shader Features
- Generates texture from heightmap (great if your procedurally generate heightmaps with say Libnoise)
- Looks good from far away to midrange
- Eight different terrain colours
- Three different detail textures: ground, water, and lights
- Control scale of detail textures
- Control metalic and smoothness of textures
- Triplanar texturing (so that textures look right regardless of angle)
- Stochastic texturing (avoids texture repition)
- Shadow attenuation (so the dark side of the planet is black)
- Control whether lights appear on the dayside or just on the darkside of the planet
- Control spread of lights
- Animate and control speed of water texture
- Control strength of heightmap and normals

Cloud Shader Features
- Input detail cloud texture for detail
- Control scale of cloud detail texture
- Control alpha threshold of cloud detail texture
- Stochastic texturing (avoids tiling of cloud detail texture)
- Shadow attenuation (so that clouds on the dark side of the planet are black)
- Triplanar texturing (so that textures look right regardless of angle)
- Animate and control speed of clouds so they move across the planet, unform and reform
- Control metalic and smoothness of clouds

![Planets03](https://user-images.githubusercontent.com/67586167/225753889-a4afaa87-05d3-4eda-85fc-a2560cb189b9.jpg)

![Planets01](https://user-images.githubusercontent.com/67586167/225753913-53899843-dff8-4a0c-82aa-bc997069b57b.jpg)

![Planets04](https://user-images.githubusercontent.com/67586167/225753926-1825333b-412c-415b-8354-2e5cd7fab181.jpg)

How To Use
- Drag the planet sphere into the scene
- Drag in your selected heightmap (the higher the resolution the better it looks)
- Fiddle around with the heightmap strength until it looks right
- Add in your ground and water and light textures (or just use the samples provided)
- If your making a desert planet or similar use the ground texture in the water slot and make sure that the water speed is set to 0 so that the ground doesn't appear to move
- Set the colours for the different heights of the heightmap
- Set what height you'd like lights to appear from... something above 0.55 is good if you dont want them to appear in the water
- 'Lights Visibility' controls the degree to which lights appear on the dayside of the planet

Credits
- I implemented the custom lighting node by Cyanilus (MIT License), which can be found here: https://github.com/Cyanilux/URP_ShaderGraphCustomLighting
- I implemented some of bgolus ideas for generating my own normal maps
- I implemented Junior_Djjr stochastic node, which can be found here: https://github.com/JuniorDjjr/UnityProceduralStochasticTexturingNode
- The cloud texture is from Solar System Scope (CC 4.0): https://www.solarsystemscope.com/textures/
- Other Textures in example files from nasa earth observatory (Public Domain)

All content is licensed under Apache 2.0 unless otherwise stated
