# EDA Render Template

This is an Unreal Engine template project for rendering out cinematic sequences for UCLA's EDA Immersive Projection System in the Broad Art Center.

[Download a ZIP file here.](https://github.com/L05/EdaRenderTemplate/archive/master.zip)

![EDA Immersive Space](http://classes.dma.ucla.edu/Spring19/24/wp-content/uploads/EDA01-1024x410.png)

The template comes with three Blueprint CineCamera Actors, one for each of the three EDA walls, and each camera has its sensor settings and transform (location, rotation, scale) preconfigured for its respective wall. The camera Blueprints can be found in *Content > EdaRender > Core*.

When you want to add a new camera to your scene, the currently recommended procedure is to drag a *BP_EdaCam_C*, a *BP_EdaCam_L*, and a *BP_EdaCam_R* into your scene from the content browser. Then, in your *World Outliner*, drag the newly created *BP_EdaCam_L* and *BP_EdaCam_R* actors onto the new *BP_EdaCam_C* so that they are now attached to it. 
<img src="Docs/WorldOutliner.png" alt="World Outliner" width="400"/>

Then reset the location and rotation to default for *BP_EdaCam_L* and *BP_EdaCam_R*.
<img src="Docs/ResetTransform.png" alt="Reset Camera Transform" width="400"/>

For reference, see the *BaseMap* and *AnimatedMap* template levels, which are located in *Content > EdaRender > Maps*.

## Relevant Tutorials and Resources

* [Rendering Out Cinematic Movies](https://docs.unrealengine.com/en-us/Engine/Sequencer/HowTo/RenderMovies)
* [Sequencer Overview](https://docs.unrealengine.com/en-us/Engine/Sequencer/Overview)
* [Cinematics with Sequencer (Video)](https://www.youtube.com/watch?v=uEnfMV-4afA&list=PLZlv_N0_O1gaiA_sfpjATUprVW7B9FcK1)
* [Render Movie or Image Sequence in Unreal Engine 4 (Video)](https://www.youtube.com/watch?v=MXluHwioBOo)
