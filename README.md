Hello, my name is Erica and I'm a masters student in computer science with specialisation in computer graphics and visualisation at KTH Royal Institute of Technology. Most of my projects are in Unity using C# and HLSL, but I have also worked with C++ as well as Java and Python. Welcome to my portfolio! Here I have gathered some of the most important things I've done in computer graphics and game development. Take a look:)

# Contact information
Email: ericat@telia.com

Links: [LinkedIn](https://www.linkedin.com/in/erica-tjernell-566669140/)

# Real-Time Volumetric Clouds in Unity
I made these clouds for a sailing game. The clouds are based on [Real-time rendering of volumetric clouds](https://www.diva-portal.org/smash/get/diva2:1223894/FULLTEXT01.pdf) by Fredrik Häggström, which is based on the work of Andrew Schneider for Horizon Forbidden West. The volume is evaluated through ray-marching. Some lighting phenomena are considered such as silver lining, through the Henyey-Greenstein phase function, and attenuation using Beer's law. 
![image](https://github.com/user-attachments/assets/f161795a-c945-409f-b164-b75282afb6d8)

<video src="https://github.com/user-attachments/assets/47225614-700a-44d9-8932-bf2bd21ad17a" controls="controls" style="max-width: 100%;"></video>

# VR asymetric collaboration maze game in Unity: "Hedged-in"
Together with a team, I created this asymetric collaboration VR game. The person in VR needs to escape from the maze, and their partner needs to guide them out by opening and closing certain walls, and luring away monsters. I was in charge of creating the hedge, which I did using shell texturing, with a custom shader using HLSL and C#. For this project we used Unity URP. My shader used GPU instancing to group the shells together and increase peformance. It was interesting to consider the difference that arises with shader programming and performance that comes with VR development.
![image](https://github.com/user-attachments/assets/1e5d1228-fbe2-4cae-94b9-55cf45613baa)
![image](https://github.com/user-attachments/assets/e746166c-9854-4e04-89b5-c20e9a1aeedd)
![hedge](https://github.com/user-attachments/assets/fd9e75f7-2d38-411d-a4b9-3386dfe8a379)

# Path/Raytracer in Unity
I have created my own custom raytracer with bounce lighting. For this project, I used Unity and a custom shader. I also implemented a BVH to increase performance, and temporal accumulation to make it less noisy.
![image](https://github.com/user-attachments/assets/39170875-df9f-41e6-83ee-001a97c0cf93)
<img width="800px" src="https://github.com/user-attachments/assets/8c05efb1-ee02-4f91-bbda-47a7807b0840">

# [Shell texturing bunny](https://stan4dbunny.github.io/Shell-Texturing/)
I have also used shell texturing for rendering fur with the Blinn-Phong shading model, but I would like to use a more sophisticated shading model in the future. Currently, the strands will not shade each other, which would improve the look. Additionally, in real life hairs are slightly transparent which can have effects such as subsurface scattering. This would be cool to implement as well.
<img width="700px" src="https://github.com/user-attachments/assets/f6228368-8caa-4f7b-9759-22f59c56419f">
<img width="700px" src="https://github.com/user-attachments/assets/7f006e3a-7460-49d5-944c-dfd906205ac0">

<video src="https://github.com/user-attachments/assets/dcef07fb-104c-45a7-8d6f-20203f5b9a8d" controls="controls" style="max-width: 100%;"></video>


# Bachelor's thesis: ["Comparison between Smoothed-Particle Hydrodynamics and Position Based Dynamics for real-time water simulation"](https://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-335984)
My bachelor's thesis was centered around comparing two implementations of two particle-based fluid simulations, in regard to performance and stability. We translated existing implementations into Unity to make a more valid comparison.
![image3](https://github.com/user-attachments/assets/388f33b4-fe1b-4415-a4a9-2237eb813a0c)


<video src="https://github.com/user-attachments/assets/0208ed69-8cb2-4cd2-98b9-3b3665c8c9a6" controls="controls" style="max-width: 100%;"></video>








