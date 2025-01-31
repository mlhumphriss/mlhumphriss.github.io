# Portfolio

## C++ Projects

### C++ Graphics Project
{% include GraphicsYoutube.html id="77X5xG5DIFI" %}
- This project was made with OpenGL used to allow it to render.
- It features real-time shadows using a shadow buffer, a shader effect which uses distance to fade into a white fog to help provide scene depth. Objects in the scene are also stored in a scene graph for more efficient rendering.
- To try and imitate realistic water physics, a sin wave is used to move the water plane and boats in a bobbing motion. This imitation is effective when looking at a small section, but is a lot less effective when you can see a large chunk of the scene.
![Scene Gif](docs/assets/MLH_Graphics_HalfTide.gif)
- A problem I had during this project was shadow acne. In order for shadows to cover the full scene from the light, I had moved it further away into the void of the edge of heightmap. Unfortunately I had forgotten to change the near plane of the projection matrix of shadow scene drawer so had an issue with depth buffer causing acne.
- Upon realising that I hadn't changed the near plane distance, I increased it and solved the problem instantly.
- If I was to revisit this project, I would try and fix the post processing as had a bug where it would render one colour across whole screen as well as adjust the water to not be as reflective
- [Github Repository](https://github.com/mlhumphriss/CSC8502-OpenGLGraphicDemo)

### C++ Physics and Ai Project
{% include GraphicsYoutube.html id="DAe-hkx5NWY" %}
- Description
- [Github Repository](https://github.com/mlhumphriss/CSC8503-NetworkCodebase)
#### OBB to OBB collisions using Separating Axis Theorem
![OBBGif](docs/assets/OBBCubesRocking.gif)
- One feature of the physics engine is an implementation of Separating Axis Theorem to work out collisions betweenv two OBB objects. This is done by projecting both onto a series of axis to check if they overlap, then using the axis which does with the least penetration to get a collision point for collision resolution.
- This method wasn't a perfect solution as after a collision, the cubes take a while to settle with them rocking on the corners
- Another issue during development was that if the objects were significantly different sizes (e.g. floor and a box) it would fling them apart
- Upon further testing I realised this occurred only when the floor was the position of Object A, so added a check that would swap any object with tag floor to Object B before the function
- Though fixing the issue inside the function would have been more ideal as would make the physics more consistent, I was under time constraint so settled on this method to fix it
- [Function Code can be seen here](https://gist.github.com/mlhumphriss/8d80fcba81a2cb78762e527afbab33c9)

### Unreal Group Gamejam - Explosive Unboxing
{% include GraphicsYoutube.html id="jw4zNAWN2P8" %}
- Description of what I worked on
![ExplosiveUnboxingSpin](docs/assets/SITDSpin2.gif)
- [Github Repository of Game](https://github.com/AlfieOnGit/ExplosiveUnboxing)

### C++ Conway's Game of Life
![ConwayWorkingGif](docs/assets/ConwayWorking.gif)
- As an introduction to C++ I was tasked with creating Conway's Game of Life with features allowing me to search seeds of an inputted size for certain patterns.
- Though it could find 4 of the 6 required patterns, it was made in 4 days while I was recovering from an illness so was inefficient and had several functions that could be easily improved
- If I was making this again with the knowledge and experience I now have, I would change a chunk of it such as the cellState function which used too many comparisons to work out the alive neighbor cells.
- [Github Repository of Codebase](https://github.com/mlhumphriss/ConwayGameOfLifeAssignment1/blob/master/main.cpp)



## Unity Projects

### Dissertation on creating an Adaptable and Efficient Autonomous Parking Syste,

### Stage 3 Games Coursework

