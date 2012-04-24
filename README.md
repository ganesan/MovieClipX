## Retina MovieClip Library
The Retina MovieClip library is exactly what the name implies, it's the MovieClip library with added support for retina displays (@2x graphics for the iPhone 4 and the new iPad) while simultaneously supporting the original non-retina devices.

## Basic Usage Tutorial
1. Make sure your `config.lua` file has this tag in it:

`imageSuffix = { ["@2x"] = 2 }`


2. Make sure you have copies of all your images, one for the high resolution graphic for the retina screen and one halfsized for old devices. You must name the files like so: 
Retina graphic = filename@2x.png
Non-Retina = filename.png
> __note: they don't have to be .png files.__


3. Now you must create a new mcx object. To create a new object use `myMCXObject = mcx.new()`
 

4. Now to animate you'll have to add a new animation to the object using `myMCXObject:newAnim("animation_name", {frames}, width, height, speed)`
> __note: you must enter the width and height of the non-retina graphic. So if the retina graphic is 128x128 you'd enter 64 for the width and height.__

5. To play one of the animations in the mcx object, use `myMCXObject:play("animation_name")`

__Extra tip: to automatically scale down your graphics for older phones use my utility MultiRezer instead of doing your sprites one by one!__
MultiRezer download: http://project239.com/multirezer


## Functions
`mcx.new()`
> Creates a new mcx object
`myMCXObject:newAnim(newAnim("animation_name", {frames}, width, height, speed)`
> Creates a new animation in an mcx object
`myMCXObject:play("animation_name")`
> Plays an animation in an mcx object
`myMCXObject:stop()`
> Stops an animation in an mcx object
`myMCXObject:currentAnimation()`
> Returns the name of the current animation


## Credits
Garet McKinley (iGARET.com)


Thanks for using the Retina MovieClip library!