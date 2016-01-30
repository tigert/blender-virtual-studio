# Blender virtual studio
A simple [Blender](http://www.blender.org) scene to explore lights and shadows with the Cycles renderer preview
Includes a few pre-defined lights and a backdrop and a simple table with a professionally
trained Test Garden Gnome. This is very quick, and there are likely other more advanced versions around, but
as I am learning Blender as I go, this is what I have so far :-)

## Overview

As blender can be a bit overwhelming for a beginner, here's a quick overview:
The scene you are loading is divided in three parts side by side: The overview,
the render preview and the "sidebar that has a lot of stuff".

### Setting things up

Load the included .blend file in Blender, and select "Cycles Render" from the top menubar 
if it is not already set. This is important for the realtime preview to work.

By default the scene has two views side by side. Each of them has a toolbar on 
the bottom side, with several selectors, a bit like this:

  ( Object Mode : ) ( @ :) ( 8 :)

The selector on the right side of "Object Mode" is the "Viewport Shading" selector. Set it
to "Rendered" on your larger preview and you should see your lights and shadows.

Set the other viewport to "Material" or "Solid" or "Wireframe". This is useful because
the render preview does not display the orange "object is selected" outline, making it
hard to see what object you are manipulating when you want to tweak colors. You can
however toggle between render preview, solid and wireframe modes with Shift-Z and Z.

## Setting Colours of lights

The scene contains no "light" objects, but rather the lights are regular 3D objects (boxes
and cylinders) that have their material set to "Emission" with a defined colour. These are
visible on the top part list of the sidebar. You can either select a light from there, or
by right clicking an object in the 3D view.

Under the list there are a number of tabs, one of which is sphere with a checkerboard.
This is the Material tab. Here you can change the color and intensity of your lights. 
You can also change the look of the Gnome if you wish, or any other objects you want
to add.

The important controls are in the "Surface" group: *Color* and *Strength*. These change
the tone and intensity of your lights. You can also scale, rotat eand move things around,
this can be achieved by dragging the colored arrows pointing away from the selected object.
The bottom toolbar has a button group where you can switch the arrows to rotation and scaling
handles too.

Note that while the *strength* setting of an emissive object directly changes the intensity
of the light, also scaling the object itself adjusts it, as the surface area of the emissive
material changes. So you need to tweak the strength if you scale lights and vice versa.

Happy exploring! :-)


