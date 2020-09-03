<meta http-equiv="refresh" content="0; URL=https://www.physicaladdons.com/psa/">

###What is Physical Starlight and Atmosphere

"Physical Starlight and Atmosphere" is a Blender addon for advanced environmental lighting that takes inspiration of 'sandbox' game world and editors like Unity or Unreal Engine. The goal of the addon is to provide high quality atmospherics and lighting and bring visual consistency between every object in your scene. As of now it is still in active development and I am working hard to make it the highest quality product.
___
###Why use it?
- very high dynamic range. Made to be used with tone mapping (filmic, or aces)
- made for PBR and HDR workflow
- consistent results - sunlight, sky and fog share the same shaders, code and parameters
- very memory efficient, does not consume video memory - works great on integrated GPUs
- performance - loads much quicker and renders faster than HDRI textures
- flexibility - simulate any planetary weather conditions 
- fully procedural - can simulate unlimited number of sky conditions
- instant results - one click away to a beautiful render
- it's yours - free to dissect the setup, re-arrange it for your needs

___
###How does it work?

This addon "fills" your Blender scene with air (or any gas of your liking) where density at the ground level is the highest and in the space - lowest, then a Star of your choice illuminates the air using physics laws - easy as that!

Lighting is calculated based on Rayleigh and Mie theory of light scattering through gaseous and liquid medium. Most critical part of the calculation is the fog - like in real world, it changes based on altitude of observer.

Although my work is based on physical functions and scientific research, my usual approach is to stick with what looks right. That's why there are some 'artistic' liberties taken (or manually fitted values based on reference images) to make it stand out from the crowd.

___
###Motivation

Outdoor lighting in is essential in computer graphics and Blender still has no proper skylight system available. Preetham and Hosek-Wilkie sky included in Blender is very rudimentary and practically unusable. Even skylight systems in other software suites are very limited.

A common practice in almost all of CG software is that components like sky, sun, fog, water, clouds, lighting is considered separate entities and they do not interact to each other. In real, physical world everything influences everything. Even bigger issue can happen when different components are created by separate teams. It causes issues where one component looks amazing and realistic, but then everything else looks off and disconnected. Then artist's responsibility is to find the issues, tweak the settings, add fake lights and other "magic" to connect the pieces back to a nice overall render. At least this has been my workflow for many years and it just felt wrong.

so...
I developed my own rendering system in GLSL for BGE (Blender Game Engine) with which I made most of my projects. It was made with PBR (Physically Based Rendering) in mind. System was time consuming to adapt to other projects so I started to play around with shader node editor. To my surprise, It was possible to "translate" most of it. And with many months of work, I managed to create a first usable version. Then a year later of constant research and optimizations I finally have this addon!

Now considering that I developed my old rendering system closely with ocean, clouds, rainbow (!) and weather system, this addon will grow into a considerable mess. This is why I am developing other components simultaneously to be later combined with atmosphere in a sensible way.

___
###Why procedural skies?

Industry is still using good old HDRI light probe method to do outdoor lighting, and for a good reason - it is the simplest way to simulate realistic lighting conditions, without worrying that it will look wrong. After all it is a 360° snapshot of a real environment.

HDRI probes unfortunately are not able to capture one crucial aspect - the fact that sky is dynamic. Sky is not just a membrane of the imaginary rim of the sky, it has volume. Sky is atmosphere and atmosphere is a physical medium consisting of a blend of gases. Sky literally starts just outside of your eyeball and extends to the outer space. Sunlight travels through this medium illuminating, scattering and absorbing in it.

procedural skies to the rescue!
Procedural skies are more common in games industry, and there the industry have developed way past the static HDRIs, skyboxes or skydomes. Just take a look at the amazing sky system for Horizon Zero Dawn

During the years I have been working with, probably, every existing atmosphere system, starting from the good old O'Neil's "Accurate Atmospheric Scattering" method, to Preetham model, Eric Bruneton's planet rendering, and Hosek-Wilkie's physical sky model. Each of them have their strengths and, unfortunately, also weaknesses. In fact, none of the existing methods proved versatile enough worth my time making an addon for Blender.

So I decided to develop a method from (mostly) a scratch - The starlight and skylight system I wish existed!

___
###Story of "Physical Starlight and Atmosphere"

This product is a result of a decade of scouting for ideal sky rendering system. I have been trying out different existing techniques and coming up with mine, but in the end never really settled on one.
It must have started with my introduction to GLSL by legendary Mike Pan. I remember bugging him with all kinds of questions. He was, probably one of the first ones who used custom GLSL scripts for Blender. I got hooked and came up with this (I can't believe it has been already 10 years!)
