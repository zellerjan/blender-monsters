## Things to add

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
    <script src="https://cdn.jsdelivr.net/gh/c-frame/aframe-extras@7.5.4/dist/aframe-extras.min.js"></script>
```
