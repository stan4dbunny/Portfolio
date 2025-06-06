Hello, my name is Erica and I'm a master's student (soon to gratuate!) in computer science with specialization in computer graphics and visualization at KTH Royal Institute of Technology. I've worked with C++, Unity using C# and HLSL, as well as Java and Python. Welcome to my portfolio! I have gathered some of the most important things I've done in computer graphics and game development. Take a look:)

# Contact information
Email: ericat@telia.com

Links: [LinkedIn](https://www.linkedin.com/in/erica-tjernell-566669140/)

# Master's thesis: Exploring global illumination with radiance caching and glossy reflections
Using AMD's graphics testing framework [Capsaicin](https://github.com/GPUOpen-LibrariesAndSDKs/Capsaicin) (C++ and GLSL), I've been exploring [GI-1.1](https://gpuopen.com/download/publications/SA2023_RealTimeReflection.pdf) and looking into improving the infinite bounce lighting approximation with the goal to improve the glossy reflections in particular. I call their original implementation singlebounce, and the improved version multibounce. 
* Worked with a codebase with an existing probe-based GI implementation
* Communicated with AMD about getting access to a work-in-progress version of multibounce that I improved
* Combined theory and application by taking the rendering equation into account when improving multibounce
* Gotten used to working with PBR and path-tracing, and compute shaders
* Used PIX and RenderDoc for debugging
* Created tool for debugging reflections by creating a reflection-only view in the path-tracer
* Tested different scenes to evaluate the impact on visual quality of multibounce compared to singlebounce (with path-tracer as ground truth), using NVIDIA's FLIP
![GI-1 1 1_Multibounce_Sponza__Main_None__165_0 019582](https://github.com/user-attachments/assets/fe3eed69-af12-48e9-881b-d4f0bad96647)
A screenshot from Capsaicin with the improved multibounce.

<video src="https://github.com/user-attachments/assets/4b98fed8-2ff2-4a71-912f-c5593f627092" controls="controls" style="max-width: 100%;"></video>
A video showing the difference between singlebounce and the improved multibounce.

# Real-Time Volumetric Clouds in Unity
I made these clouds for a sailing game. The clouds are based on [Real-time rendering of volumetric clouds](https://www.diva-portal.org/smash/get/diva2:1223894/FULLTEXT01.pdf) by Fredrik Häggström, which is based on the work of Andrew Schneider for Horizon Forbidden West. Things I did in the project:
* Created tool to easily create, view, debug, and update 3D noise texture assets using a compute shader and Unity's scripted importer feature
* Implemented ray-marching in a shader for density evaluation and lighting contribution
* Considered real-life lighting phenomena such as in/out scattering with the Henyey-Greenstein phase function, and attentuation using Beer's law
* Did a parameter study where I varied the step size to balance visual quality and performance
![image](https://github.com/user-attachments/assets/f161795a-c945-409f-b164-b75282afb6d8)
A screenshot of the clouds with "maximal" visual quality settings
<video src="https://github.com/user-attachments/assets/47225614-700a-44d9-8932-bf2bd21ad17a" controls="controls" style="max-width: 100%;"></video>
A video showcasing the clouds with a day-and-night cycle to show how the light affects the clouds.

# VR asymetric collaboration maze game in Unity: "Hedged-in"
Together with a team, I created this asymetric collaboration VR game. The person in VR needs to escape from the maze, and their partner needs to guide them out by opening and closing certain walls, and luring away monsters. In this project I focused on creating the material for the hedge with shell texturing.

* Implemented GPU instancing to group the "shells" (layers) to improve performance
* Adapted the shader to work for stereo rendering (VR)

![image](https://github.com/user-attachments/assets/1e5d1228-fbe2-4cae-94b9-55cf45613baa)
A picture of a play test of the game. Although it's a bit blurry, the hedge and the shell texturing which gives it its bushy look can be seen on the TV screen. 

# [Shell texturing bunny](https://stan4dbunny.github.io/Shell-Texturing/)
I have also used shell texturing to create fur. Click the link above if you want to read more about it and try out the interactive demo! The project included:
* Fur placement and length based on grayscale texture created in Blender
* Fur color based on any texture
* Strands that move when the bunny moves through vertex displacement
* Blinn-Phong shading
* Simple controls to move and rotate bunny
<img width="700px" src="https://github.com/user-attachments/assets/f6228368-8caa-4f7b-9759-22f59c56419f">

A screenshot of a bunny with shell textured fur. Note the lack of fur on the eyes and in the ears. 

<img width="700px" src="https://github.com/user-attachments/assets/7f006e3a-7460-49d5-944c-dfd906205ac0">

A screenshot where the layered nature of the technique is visible.

<video src="https://github.com/user-attachments/assets/dcef07fb-104c-45a7-8d6f-20203f5b9a8d" controls="controls" style="max-width: 100%;"></video>

A video from the interactive demo where it can be seen that the fur strands move when the bunny is moved back and forth. 

# Path-tracer in Unity
I implemented a simple GPU path-tracer using a shader with:
* An axis-aligned bounding volume hierarchy (BVH) to make ray traversal more efficient and improve performance
* Temporal accumulation, denoising the render over time
![image](https://github.com/user-attachments/assets/39170875-df9f-41e6-83ee-001a97c0cf93)

A screenshot of Cornell Box rendered with my path-tracer. Note the bounce-lighting.

<img width="800px" src="https://github.com/user-attachments/assets/8c05efb1-ee02-4f91-bbda-47a7807b0840">

A screenshot of how the BVH works.

# Bachelor's thesis: ["Comparison between Smoothed-Particle Hydrodynamics and Position Based Dynamics for real-time water simulation"](https://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-335984)
My bachelor's thesis was centered around comparing two implementations of two particle-based fluid simulations, in regard to performance and stability. With a partner, I ported existing implementations into Unity to make a more valid comparison.
![image3](https://github.com/user-attachments/assets/388f33b4-fe1b-4415-a4a9-2237eb813a0c)

A screenshot from one of the simulations where water from two directions has crashed into each other. 

<video src="https://github.com/user-attachments/assets/0208ed69-8cb2-4cd2-98b9-3b3665c8c9a6" controls="controls" style="max-width: 100%;"></video>

A video of one of the simulations where it can be seen how water from two directions crashes into each other and dissipates.







