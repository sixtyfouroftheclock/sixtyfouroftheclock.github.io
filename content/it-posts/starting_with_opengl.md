---
title: "Starting with OpenGL"
date: 2025-12-08
lastmod: '2025-12-12'
description: "We're gonna learn about OpenGL in this article!"
tags: ['c', 'cpp', 'opengl']
---

(I am still updating this article. I wanna make it simple, understandable)

Hello, again.

# Whatta heck is OpenGL?

## Easy way

OpenGL is a software that lets programmers play with graphics directly easily. Allowing creating
programs like Blender[^blenderrequirements], FreeCAD[^freecadopengl], or games, such as Minecraft[^minecraftrequirements].
Itself is just a specification[^openglspecification] - mostly implemented in your graphics card driver.

If your graphics card and its driver supports OpenGL 3.3, it CAN NOT be upgrade or run OpenGL 4.6 using the native way[openglcantupgrade].
Because, 4.6 version is, in a way, "burnt" to the graphics card[graphics_card_instructions]. You can emulate it, but it's gonna lose performance.

This is the top information about OpenGL. OpenGL is complex, not as much as [vulkan](https://vulkan.org/), but it still is.

## Hard way

OpenGL is a specification[^openglspecification] which lets you control.

Graphics card drivers read its instructions and translate them into something programmers can use easily.

That means, in another words,


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
[openglcantupgrade]: No reference yet
[graphics_card_instructions]: https://en.wikipedia.org/wiki/Instruction_set_architecture
