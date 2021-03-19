# Entry 3
##### 3/15/21
# Sources 
<p>Over the months, I've been doing close research and kinda envisioning a rough draft of how I'm going to execute my freedom project of creating a 3D model where the user can select from a dropdown menu of what they wanted to display on the screen. I came across mutiple videos and resources on the Babylon.js but the one that struck out to me was the video called,<a href="https://www.youtube.com/watch?v=XFT5omp_F3g"> Babylon.js Tutorial Series - Part 1: Getting Started</a>, where they also have a series of video where they explains the different components that goes into making a Babylon.js. I also tried many examples on Repl with attempting to use Babylon.js, but the examples failed miserably.</p>
<br>
<p> In addition, to the video introducing the beginning to making a Babylone.js program. I also found this cool program up on Babylon.js called,<a href="https://www.babylonjs-playground.com/#6F0LKI#1"> Babylon.js Playground 5.0.0-alpha.14 (WebGL)</a>, where it was a set up to a program that operates on a free camera which it targets the scene origin. It began by creating a scene where the Babylon.js can take place and slowly positioning the camera at a fix postion so the user can move around the object around freely. In this code snipet, it is of a red ball placed on top of a surface:</p>
  
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
   <p> I am now currently between Stage 4 and 5 of the Engineering Design Process: Plan the most promising solution and Create a prototype. This is because I have already thought or attempt to thought of possible solutions to my errors and already tested some out. I am starting to plan the most efficent code or solutions to go in my Freedom Project from what I learn already about APIs and database to loops and conditionals. I'm pretty much in the process where I'm ready to begin creating my Babylon.js prototype project and picking up ideas along the way. Thoughout the Create a prototype or Stage 5, I'll try to learn more through research and throughout class about DOM to help me better understand Babylon.js. I also trying this cool idea of mine to try 3D model where the camera postion is 360 degrees so the user can go around the object without just one singular camera position which I'll try my best to accomodate.</p>
   <br>
   <p> On Stage 5, I'll try to try something light like using only one camera position, focusing only on one object and until the next entry I'll slowly applying what I can learn about 360 Photo Domes and 360 Video Domes and slowly adding in more shapes and object to the surrounding and we go from there. After I completed Stage 5 to Create a prototype, I try to Test and evaluate the prototype by removing any bugs or testing the functionality of the project. By the end of the Freedom Project, I want a website that can view anything in 360 environments provided by the dropdown menu.</p>
 
 # Knowledge
  <p>  From the youtube video, <a href="https://www.youtube.com/watch?v=Cib3Y64GVWE"> BabylonJS Tutorial Series -- Part 2: Cameras</a>, to the cool page, <a href="https://doc.babylonjs.com/divingDeeper/cameras/camera_introduction"> Camera Introduction</a> at the Babylon.js page. I learned how the different camera format can effect the user's overall experience and how powerful Babylon.js really is, is unbelievable.</p> 
  <br>
  <p> I learned that an Arc Rotate Camera is a camera that always points towards a given target position and can be rotated around that target with the target as the center of rotation. It can be controlled with cursors and mouse, or with touch events. View it like this, this is the exact camera position that is being used in <a href="https://earth.google.com/web/@59.373245,-100.2579411,-19507.5501395a,22271260.42582512d,35y,0h,0t,0r"> Google Earth.</a> This camera is orbiting around the target position like a satellite that orbits the Earth whihc can be set by three parameters: alpha (the longitudinal rotation, in radians),
beta (the latitudinal rotation, in radians), and radius (the distance from the target).

    Parameters: name, alpha, beta, radius, target position, scene
    var camera = new BABYLON.ArcRotateCamera("Camera", 0, 0, 10, new BABYLON.Vector3(0, 0, 0), scene);
    
    // Positions the camera overwriting alpha, beta, radius
    camera.setPosition(new BABYLON.Vector3(0, 0, 20));
    
    // This attaches the camera to the canvas
    camera.attachControl(canvas, true); 
 <p> This is just one of the many cool camera format others includes: Universal Camera, Follow Camera, Anaglyph Cameras, Device Orientation Camera, Virtual Joysticks Camera, and etc. By understanding how the camera works in Babylon.js, I am able to come up with more interesting ideas and concepts for my Freedom Project. The camera is just one of the component to make a cool fundamental Babylon.js project.</p>
 
 # Skills
 <p> The skills I think I honed during the process was Problem decomposition: breaking a task down into smaller pieces and Creativity: how to think outside the box, be innovative, and create the future.
 <p> I think I was able to develop my Problem decompositon skill because decomposing down a problem and retracing your steps back to the beginning and going from there is a skill that take patient and lot of attention and is not easy. For example, for this Blog Entry my problem at the beginning of the Entry was how was I able to start or create using Babylon.js to build a camera set. I was disecting down my purpose for Babylon.js until I got to the core issue and got a clear sense of what was I trying to do, find how to use a camera in Babylon.js and a I guess a moveable target.</p>
 <p> Another skill I picked up during the process was my Creativity. Personally, I am not a very creative person who happens to be stubborn and clumsy. Being able to know enough about Babylon.js and how it works and it's gear, allows me to be more prone to many ideas and thoughts coming my way. For example, while researching about camera positions, I was much more susceptible to the different camera format and the different way I can apply it to my own Freedom Project
 



  
    

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
