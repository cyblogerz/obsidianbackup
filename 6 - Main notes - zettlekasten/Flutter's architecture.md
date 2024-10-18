Date: 2024-10-14     Time: 01:40

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status: #baby

Tags : [[flutter]]

# Flutter's architecture
The flutter's architecture consists of three layers :
- ***Framework(dart)***
- ***Engine(c/c++)***
- ***Embedder(platform specific)***

![[Pasted image 20241014014243.png]]




- Flutter has a modular architecture .Allows you to write the application logic once and have consistent behaviour across different  platforms. 

## The framework layer
[[The framework layer]]
- This layer is written in dart and it is responsible for building the ui . it contains the high level library that we directly use to build the app.  This includes the UI theme, widgets, layout and animations, gestures and foundational building blocks.

- In the framework layer alongside the framework there is a plugin's layer - it controls high level features like access to geo location,  camera, in app payments, etc.

## Engine layer
- It contains the c++ libraries makes up the primitives that supports the flutter apps . 

> [!NOTE]
> - Primitives here refer to the basic building blocks or low level functionalities provided by the c ++ libraries that flutter uses to build more complex features
> 
> - The primitives includes - memory management, threading, file handling, or networking.
> 
> - Example : flutter depends on c++ primitives to handle drawing operations on the screen , manage low level hardware interactions.
> 
> 

 -  The engine is also responsible for **rasterizing** Flutter scenes for fast rendering onscreen.
-  It provides the low-level implementation of Flutter's core API, including graphics (through [Impeller](https://docs.flutter.dev/perf/impeller) on iOS and coming to Android and macOS, and [Skia](https://skia.org/) on other platforms)

##### Rasterizing :
 - In computer graphics rasterization means - 
 - In [computer graphics]  **rasterization**  is the task of taking an  image described in a vector graphics format (shapes) and converting it into a raster image (a series of [pixels](https://en.wikipedia.org/wiki/Pixel "Pixel"), dots or lines, which, when displayed together, create the image which was represented via shapes).
 
 - The rasterized image may then be displayed on a [computer display](https://en.wikipedia.org/wiki/Computer_display "Computer display"), [video display](https://en.wikipedia.org/wiki/Video_display "Video display") or [printer](https://en.wikipedia.org/wiki/Computer_printer "Computer printer"), or stored in a [bitmap](https://en.wikipedia.org/wiki/Bitmap "Bitmap") file format. Rasterization may refer to the technique of drawing [3D models](https://en.wikipedia.org/wiki/3D_model_(computer_graphics) "3D model (computer graphics)"), or to the conversion of 2D [rendering primitives](https://en.wikipedia.org/wiki/Rendering_primitive "Rendering primitive"), such as [polygons](https://en.wikipedia.org/wiki/Polygon "Polygon") and [line segments](https://en.wikipedia.org/wiki/Line_segment "Line segment"), into a rasterized format.


## Embedder
1. The **Embedder** is different for each target platform and handles packaging the code as a stand-alone app or embedded module.

![[Pasted image 20241014184159.png]]****

---


> [!NOTE]
> ###### Each of the layer is made up of other sub layers and modules , making them almost fractal . 
> 

 The reason this architecture is often described as “fractal” is because each layer, while interacting with other layers, is composed of smaller reusable components that have their own sub-modules or classes.
 

# References
Similar notes and source ideas

[Kodeco - flutter blog](https://www.kodeco.com/books/flutter-apprentice/v1.0/chapters/1-getting-started#toc-chapter-008-anchor-003)
