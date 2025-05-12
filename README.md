# :rocket: 3D Monster-World

## How to Experience It
https://zellerjan.github.io/blender-monsters/ <br>
Open the VR environment in a supported Browser or your VR-Headset. Explore the monster exhibition and admire the creativity!


## About
This project was created within three days as part of a learning experience with our apprentices. The goal was to introduce them to Blender and 3D modeling, allowing them to design their own monsters from scratch. Each apprentice crafted a unique 3D creature, which is now showcased in a fully VR-compatible world. The project demonstrates the rapid learning curve and creative potential of beginners in 3D design and virtual reality development.



## Dev Notes
Things to add to the Repo after Export with aFrame Plugin:
1. Library for Movement-Support
```
<script src="https://cdn.jsdelivr.net/gh/c-frame/aframe-extras@7.5.4/dist/aframe-extras.min.js"></script>
```

2. Controls and Hands for Movement
```
<a-scene shadow="type: pcfsoft; autoUpdate: false;" renderer="antialias: false; colorManagement: false; physicallyCorrectLights: false;">
      <a-entity id="rig" movement-controls="controls: gamepad,keyboard,nipple" nipple-controls="mode: static">
            <!-- camera -->
            <a-entity camera position="0 1.6 5" look-controls="pointerLockEnabled: true">
            </a-entity>
      
            <!-- hands -->
            <a-entity hand-controls="hand: left"></a-entity>
            <a-entity hand-controls="hand: right"></a-entity>
      </a-entity> 
```

3. Environment: Light + Sky Color
```
  <!-- Lights -->
  <a-entity position="50.71441650390625 27.212543487548828 26.844383239746094"
      light="castShadow:true; color:#ffffff; distance:40.0; type:directional; intensity:1.0; shadowBias: -0.001; shadowCameraFar: 501.02; shadowCameraBottom: 12; shadowCameraFov: 101.79; shadowCameraNear: 0; shadowCameraTop: -5; shadowCameraRight: 10; shadowCameraLeft: -10; shadowRadius: 2;"></a-entity>
  <a-entity position="-43.60400390625 27.212543487548828 26.844383239746094"
      light="castShadow:true; color:#ffffff; distance:40.0; type:directional; intensity:1.0; shadowBias: -0.001; shadowCameraFar: 501.02; shadowCameraBottom: 12; shadowCameraFov: 101.79; shadowCameraNear: 0; shadowCameraTop: -5; shadowCameraRight: 10; shadowCameraLeft: -10; shadowRadius: 2;"></a-entity>
  <a-entity position="0.0 17.71710968017578 -22.140750885009766"
      light="castShadow:true; color:#ffffff; distance:40.0; type:directional; intensity:1.0; shadowBias: -0.001; shadowCameraFar: 501.02; shadowCameraBottom: 12; shadowCameraFov: 101.79; shadowCameraNear: 0; shadowCameraTop: -5; shadowCameraRight: 10; shadowCameraLeft: -10; shadowRadius: 2;"></a-entity>
  <a-entity position="0.0 100.93122100830078 -53.383304595947266"
      light="castShadow:true; color:#ffffff; distance:40.0; type:directional; intensity:1.0; shadowBias: -0.001; shadowCameraFar: 501.02; shadowCameraBottom: 12; shadowCameraFov: 101.79; shadowCameraNear: 0; shadowCameraTop: -5; shadowCameraRight: 10; shadowCameraLeft: -10; shadowRadius: 2;"></a-entity>

  <!-- Sky -->
  <a-sky color="#FFF"></a-sky>
```

4. Set Rendering True
```
renderer="antialias: true;
```
