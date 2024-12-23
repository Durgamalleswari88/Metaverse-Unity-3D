Overview:
This Unity project enables dynamic interaction between objects and the camera within a 3D scene. Using three custom scripts, it allows users to change the camera's target, adjust the field of view dynamically, and rotate objects around a target.

Features:
-Dynamic Camera Target:
Click on objects to make the camera focus on them.
Adjusts the camera's field of view based on the object's size.
-Camera LookAt Functionality:
Continuously makes the camera look at a specified target.
Allows dynamic updates to the target at runtime.
-Object Rotation:
Rotates objects around a target at a configurable speed.
Defaults to rotating around the object's parent if no target is assigned.

Scripts
-ChangeLookAtTarget.cs:
Handles mouse click events on objects.
Updates the camera's target and adjusts the field of view dynamically.
-LookAtTarget.cs:
Ensures the camera always looks at the specified target.
Updates the orientation in real-time.
-RotateAround.cs:
Rotates objects around a target object at a specified speed.
Defaults to the parent GameObject if no target is provided.

Setup Instructions
-Step 1: Add Scripts to Your Unity Project
   Create a folder named Scripts in your Unity project.
   Add the following scripts as .cs files:
      ChangeLookAtTarget.cs
      LookAtTarget.cs
      RotateAround.cs
   Copy the respective script contents into each file.
-Step 2: Configure the Scene
   Set Up the Camera:
     Add a camera to your scene.
     Attach the LookAtTarget script to the camera.
   Add Objects for Interaction:
     Create or import 3D objects (e.g., spheres, cubes).
     Attach the ChangeLookAtTarget script to the objects you want to interact with.
  Optional: Add Rotation:
     Attach the RotateAround script to objects you want to rotate.
     Configure the speed parameter in the Inspector for desired rotation speed.
     Assign a target (optional).
-Step 3: Play the Scene
     Enter Play mode.
     Click on objects to make the camera focus on them.
     Observe objects rotating if the RotateAround script is used.

