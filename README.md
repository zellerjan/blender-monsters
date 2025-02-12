# 3D Monster-World

## How to Experience It
https://zellerjan.github.io/blender-monsters/
Open the VR environment in a supported Browser or your VR-Headset. Explore the monster exhibition and admire the creativity!


## About
This project was created within three days as part of a learning experience with our apprentices. The goal was to introduce them to Blender and 3D modeling, allowing them to design their own monsters from scratch. Each apprentice crafted a unique 3D creature, which is now showcased in a fully VR-compatible world. The project demonstrates the rapid learning curve and creative potential of beginners in 3D design and virtual reality development.



### Dev Notes
```
<script src="https://cdn.jsdelivr.net/gh/c-frame/aframe-extras@7.5.4/dist/aframe-extras.min.js"></script>
```
```
<a-scene shadow="type: pcfsoft">....
```
```
<a-entity
      id="rig"
      movement-controls="controls: gamepad,keyboard,nipple"
      nipple-controls="mode: static"
    >
      <!-- camera -->
      <a-entity
        camera
        position="0 1.6 5"
        look-controls="pointerLockEnabled: true">
      </a-entity>
 
      <!-- hands -->
      <a-entity hand-controls="hand: left"></a-entity>
      <a-entity hand-controls="hand: right"></a-entity>
    </a-entity>
```


```
<a-light type="directional" color="#fff2cc" intensity="0.8"position="3 5 -2" castShadow="true"></a-light>
<a-light type="ambient" color="#ddd" intensity="0.4"></a-light>
```
