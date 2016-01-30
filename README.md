# Blender virtual studio
A simple [Blender](http://www.blender.org) scene to explore lights and shadows with the Cycles renderer preview
Includes a few pre-defined lights and a backdrop and a simple table with a professionally
trained Test Garden Gnome. This is very quick, and there are likely other more advanced versions around, but
as I am learning Blender as I go, this is what I have so far :-)

As blender can be a bit overwhelming for the first time user, here's a quick overview
to get you started. The scene you are loading is divided in three parts side by side. 
There are two 3D views, and a sidebar with a lot of stuff.

### Setting things up

Load the included .blend file in Blender, and check that you have the "Cycles Render" selected on the 
top menubar.

The scene has two views side by side. Each of them has a toolbar on the bottom with
several selectors, a bit like this:

  ( Object Mode : ) ( @ :) ( 8 :)

The selector on the right side of "Object Mode" is the "Viewport Shading" selector. Set it
to "Rendered" on your larger preview and you should see your lights and shadows.

Keep the other viewport as-is (either "Material" or "Solid" or "Wireframe") because
the actual render preview does not display the orange "object is selected" outline, 
making it difficult to know what object you have selected. You can also toggle between
render preview, solid and wireframe modes with Shift-Z and Z for the viewport under 
your mouse pointer.

## Setting colours and intensities of lights

The scene currently contains no specific "light" objects, but rather the lights are
regular 3D objects (boxes and cylinders) that have their material set to "Emission"
with a defined colour. These are visible on the top part list of the right sidebar.
You can either select objects by clicking them on the list, or by right clicking any
object in the 3D view.

Under the list there are a number of tabs, one of which is Material, sphere with a 
checkerboard as its icon. Here you can change the color and intensity of your lights. 
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

If you need inspiration for the actual lighting setups, see
www.strobist.com for a great set of learning material.

