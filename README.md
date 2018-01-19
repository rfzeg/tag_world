# tag_world

This package contains models needed to simulate tags that are used for visual
tracking. To create the files I used blender and did the following:

- Download newest [Blender](https://www.blender.org/download/) (I'm using 2.79)
- Open blender
- Open the world tab on the right. 
- Select Environmental Lighting
- Change from Object Mode to Edit Mode in the bottom left toolbar (tab)
- Change from vertex selection to face selection in the bottom toolbar (ctrl tab)
- Select a face (right click)
- Unwrap (U->unwrap)
- Select material tab from the circle tab on the right
- Click the plus to add a new material slot
- Click New to create a new material
- Click Assign to assign the material to the face
- Change to the texture tab (right of the circle tab)
- Create a new one
- Change Type to 'Image or Movie'
- Under 'Image' select Open
- Select your image
- Hit F12 to render the image and see the texture
- Hit ESC to exit the rendering
- Repeat until all faces have their own materials with textures
- Click the top left icon and select Info
- File->Export (Collada .dae)
- Open the saved .dae file.
- Edit 'ambient' values to be 1 1 1 1
- Edit lines to: <texture texture="tag0_no_border__png-sampler" texcoord="UVMap"/>  
    
Hopefully you don't need to do that, as the .dae files can be edited to replace
the images, as well as to resize the tag. 
