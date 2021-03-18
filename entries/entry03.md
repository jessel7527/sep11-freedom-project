# Entry 3
##### 3/15/21
# Sources
<p>Over the months, I've been doing close research and kinda envisioning a rough draft of how I'm going to execute my freedom project of creating a 3D model where the user can select from a dropdown menu of what they wanted to display on the screen. I came across mutiple videos and resources on the Babylon.js but the one that struck out to me was the video called,<a href="https://www.youtube.com/watch?v=XFT5omp_F3g"> Babylon.js Tutorial Series - Part 1: Getting Started</a>, where they also have a series of video where they explains the different components that goes into making a Babylon.js. I also tried many examples on Repl with attempting to use Babylon.js, but the examples failed miserably.</p>
<br>
<p> In addition, to the video introducing the beginning to making a Babylone.js program. I also found this cool program up on Babylon.js called,<a href="https://www.babylonjs-playground.com/#6F0LKI#1"> Babylon.js Playground 5.0.0-alpha.14 (WebGL)</a>, where it was a set up to a program that operates on a free camera which it targets the scene origin. It began by creating a scene where the Babylon.js can take place and slowly positioning the camera at a fix postion so the user can move around the object around freely. In this code snipet, it is of a red ball placed on top of a surface:
  
     var createScene = function () {

    //This creates a basic Babylon Scene object (non-mesh)
    var scene = new BABYLON.Scene(engine);

    //This creates and positions a free camera (non-mesh)
    var camera = new BABYLON.FreeCamera("camera1", new BABYLON.Vector3(0, 5, -10), scene);

    //This targets the camera to scene origin
    camera.setTarget(BABYLON.Vector3.Zero());

    //This attaches the camera to the canvas
    camera.attachControl(canvas, true);

    // This creates a light, aiming 0,1,0 - to the sky (non-mesh)
    var light = new BABYLON.HemisphericLight("light", new BABYLON.Vector3(0, 1, 0), scene);

    // Default intensity is 1. Let's dim the light a small amount
    light.intensity = 0.7;
    light.diffuse = BABYLON.Color3.Red();
    // Our built-in 'sphere' shape.
    var sphere = BABYLON.MeshBuilder.CreateSphere("sphere", {diameter: 2, segments: 32}, scene);

    // Move the sphere upward 1/2 its height
    sphere.position.y = 1;

    // Our built-in 'ground' shape.
    var ground = BABYLON.MeshBuilder.CreateGround("ground", {width: 6, height: 6}, scene);

    return scene;

    };
   # Engineering Design Process(EDP)


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
