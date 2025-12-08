---
title: "Starting with OpenGL"
date: 2025-12-08
description: "We're gonna learn about OpenGL in this article!"
tags: ['c', 'cpp', 'opengl']
---

Hello, again.

# Whatta heck is OpenGL?

If this post reached you, probably it's because you wanna learn OpenGL, or you don't know what this word means.
OpenGL lets programmers mess with graphics. Allowing creating,
programs like Blender[^blenderrequirements], FreeCAD[^freecadopengl], or games, such as Minecraft[^minecraftrequirements].

Itself is just a specification[^openglspecification], a standard. That means, in another words,
"HEY! WE, FROM KHRONOS[^khronos], HAVE CREATED THIS PROJECT CALLED OPENGL!
IT'S FREE! BUT YOU HAVE TO IMPLEMENT IT FOR YOUR GRAPHICS CARD!". Then, the OS have to find all the OpenGL's function addresses.

# Using OpenGL with C/C++ (for programmers)

The "classic way" to create programs with OpenGL is using a bunch of libraries implemented in C or C++[^openglmainimplementationlanguage].

The simplest way to create a program in OpenGL and C is creating a native window,
then creating and making the context current. That means, it displays nothing,
just a black and boring window... Let's paint it blue using an OpenGL function!

This little program is going to need 2 libraries. A library for window management; displaying a window, closing it, handling mouse and keyboard I/O.
And another for OpenGL functions, painting the window, creating triangles, and more.

There are a bunch of libraries for creating a window. Such as [GLFW](https://www.glfw.org/) or [SDL](https://www.libsdl.org/). Let's use GLFW, because it's used for OpenGL stuff.

```bash
$ sudo apt update && sudo apt install libglfw3-dev libglew libglew-dev
```

```c

// todo

#include <GLFW/glfw.h>
#include <GL/glew.h>

int main()
{
    return 0;
}
```

To be continued. Too tired.

[^minecraftrequirements]: Minecraft requirements for 2025 https://help.minecraft.net/hc/en-us/articles/30298767427597-Operating-System-Sunset-Announcements-for-Minecraft
[^blenderrequirements]: Blender requirements https://www.blender.org/download/requirements
[^openglspecification]: Missing source from Khronos, but search later.
[^khronos]: The organization behind OpenGL. https://khronos.org/
[^freecadopengl]: FreeCAD Display settings shows use OpenGL instead of CPU https://wiki.freecad.org/Preferences_Editor#Display
[^openglmainimplementationlanguage]: Most of times OpenGL is implemented in C (missing source)
