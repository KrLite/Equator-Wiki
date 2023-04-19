---
description: The foundation to all.
---

# Vectors and Boxes

**Box** is the basic for everything in 2D rendering, and **Vector** is what that forms a **Box.**

## Why Box?

In 2D rendering and especially in Minecraft, a non rotatable rectangle is all that needed to declare the size and position to render. In order to be simple, all the transforms on rotations are embedded into the Quaternion, which the MatrixStack also uses.
