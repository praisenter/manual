---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Slides
date: 2025-11-03 09:48:58 -0500
relpath: ../
---

# Slides
> Slides are the backbone of presenting content in Praisenter - you can't present anything without a slide.
{: .p-man-page-intro}

Slides are canvases where you can add content like bible verses, song lyrics and media.  Slides fall into two categories in Praisenter, _slides_ and _slide templates_.  Slides are just what you would imagine, a canvas to place static text and media, very similar to PowerPoint or similar applications.  Slide templates have all the same features as slides, but allow for placeholder content that will be replaced on-the-fly when you are presenting.

> Praisenter doesn't support import of slides from another application at this time.

A slide is made up of the slide itself and components.  Components are things like blocks of text or images and video.  Slides and components share some common properties like backgrounds, but components have a little more customizability.

For this part of the manual, we're going to start with the fundamentals first like choosing colors and gradients, then continue to build on those fundamentals, and concluding with describing the types of components.

## Opacity / transparency[#](#opacity--transparency)
Opacity is the measure of how transparent something is.  Here's a good way to think of opacity:
- A wall in your house has an opacity of 100% because you cannot see through it at all, it's completely opaque.
- A window in your house has an opacity of 0% because you can see right through it, it's completely transparent.
- A tinted window on your car has an opacity somewhere between 0% and 100% because you can see through it, but it's _tinted_ or colored.

You can use opacity to achieve blending of content like components, media, and colors.  When making something fully or partially transparent, you will see something like the following.  The checkerboard pattern of grey and white squares show to indicate that the element is partially or completely transparent.

> NOTE: Praisenter allows you to create slides that are completely transparent.  The content of that slide will blend with whatever is in the background, whether that be a desktop background, another application, a video playing, and so on.

![Slides transparency]({{ page.relpath }}assets/img/slides-transparency.png){: .rounded .img-fluid}

## Colors[#](#colors)
Many options of a slide involve choosing a color - backgrounds, text color, borders, and so on.  Color is a fundamental element of slide editing so knowning how to select a color is important.  When selecting a color, Praisenter gives you a default palatte of colors to choose from. To choose a color, click on the color you want to use.

You aren't limited to the colors in the default palette.  Click the "Custom Color" link to open the custom color dialog.  The custom color dialog allows you to create your own color in HSB, RGB, or Web mode.  You can also specify the (also known as transparency).  Use the mouse to drag the circle around in the large square on the left to choose the saturation and brightness.  Drag the vertical slider to change the hue.

![Slides color palette]({{ page.relpath }}assets/img/slides-color-palette.png){: .rounded .img-fluid .float-start .pe-4}
![Slides custom color selector]({{ page.relpath }}assets/img/slides-custom-color.png){: .rounded .img-fluid}

## Gradients[#](#gradients)
A gradient is type of coloring that uses two or more colors and blends those colors into each other.  Praisenter supports two-stop linear or radial gradients.  When configuring the gradient you can specify the color locations using the mouse to click and drag the circles in the preview square.  

The cycle option allows you have the gradient repeat.  To see the effect, move one of the circles in the preview square.

The offset controls determine how long to use 100% of the color of the stop before starting to blend.

![Slides gradient selector]({{ page.relpath }}assets/img/slides-gradient.png){: .rounded .img-fluid}

## Media[#](#media)
Media is general term used in Praisenter to group images, pictures, audio, and video.  To use media on a slide, you must _import_ that media first.  To import media drag-n-drop the file onto the Praisenter application or use the `File` -> `Import` menu option.  Some media (audio and video) will be converted to a supported format during the import.  You can see the progress of the import in the bottom bar of the application or on the Tasks tab.

When choosing a media item, you have additional settings depending on the type of media:

| Option | Image | Audio | Video | Notes |
|---|---|---|---|---|
| Tile image | ✓ | | | Repeat the image to fill the whole space |
| Scaling | ✓ | | ✓ | None (don't change size), stretch, or keep aspect ratio |
| Adjust color | ✓ | | ✓ | Adjust the color of the content |
| Loop? | | ✓ | ✓ | Whether to restart the media when it finishes playing |
| Mute? | | ✓ | ✓ | Whether to mute the audio |
{: .table .w-auto}

### Color adjust
Color adjustment is available to both images and video.  This feature allows you to alter the colors of an image on the fly without using an image or video editor.  Want the content darker or lighter?  Use the brightness and contrast sliders.  Found the perfect asset, but you want it green instead of purple?  Use the hue slider.

![Slides color adjust]({{ page.relpath }}assets/img/slides-color-adjust.png){: .rounded .img-fluid}

## Backgrounds / borders[#](#backgrounds--borders)
Both the slide itself and every component supports a background.  Backgrounds are painted under the content.  A background can be None (transparent), a Color, a Gradient, an Image, or a Video.  Slides and components can only have one background.

Similarly, both the slide and every component supports borders.  Borders wrap around the edge of the element.  Borders are also available on text.  Borders can be None (no borders), a Color, or a Gradient.  You can adjust the border width, style, and radius.

- Line cap - The style of the border when the border ends
- Line join - The style of the border when the border turns
- Dash pattern - The style of the border lines themselves.  This will scale with the border width.

![Slides border]({{ page.relpath }}assets/img/slides-border.png){: .rounded .img-fluid}

## Shadow / glow[#](#shadow--glow)
Shadow and glow are two sides of the same coin.  They both use a color and spread it from the element outward to transparency.  Shadowns and glow can create the illusion of depth and texture.  When you enable shadow or glow, you can control these properties to produce the effect you are looking for.

> Only components and text support shadow and glow.

- The Type allows you to create an inner or outer shadow/glow.
- The `X` and `Y` offset determine how far from center
- The Radius controls how far from the element to end
- The Spread controls how much radius will be 100% of the chosen color

![Slides shadow and glow]({{ page.relpath }}assets/img/slides-shadow-glow.png){: .rounded .img-fluid}

## Font / padding / fill[#](#font--padding--fill)

