# fract-ol
I have discovered the 2D programming and the psychedelic universe of fractals 

`fract-ol` is a graphical project from the 42 curriculum focused on rendering mathematical fractals in real time using the MiniLibX library.

The program displays fractal sets such as Mandelbrot and Julia, allowing interactive exploration through zooming.

## Result

✅ Final Grade: **100/100**

---

# Project Overview

The goal of this project is to render fractal sets using complex number mathematics while ensuring smooth real-time interaction and efficient rendering.

This project demonstrates:
- mathematical visualization
- event-driven programming
- low-level graphics handling
- performance optimization in C
- interaction with the Linux graphical stack

---

# Features

- Mandelbrot set rendering
- Julia set rendering
- Real-time zoom
- Smooth graphical output
- Efficient pixel rendering

---

# Linux / Graphical System Context

This project runs in a Linux graphical environment based on the **X Window System**, which is the foundation of graphical interfaces on Unix-like systems.

## X Window System (X11)

The X Window System provides the core infrastructure for graphical applications on Linux. It is responsible for handling:
- screen drawing
- keyboard input
- mouse input
- window creation and events

In modern Linux systems, the GUI is modular and follows a **client-server architecture**, where applications communicate with the display server.

## X Server

The **X server** is the heart of the graphical system.

Common implementations include:
- **X.Org Server** (default on most Linux distributions)
- historical: **XFree86** (used before ~2004)

The X server is responsible for:
- rendering graphics
- managing input devices (mouse, keyboard)
- communicating with applications

## Window Manager

The X server only provides drawing capabilities — it does not manage window behavior.

That role is handled by a **Window Manager**, which defines:
- window appearance
- placement
- resizing behavior
- focus and decorations

Examples include:
- **KWin** (KDE)
- **Metacity / Mutter** (GNOME)
- **FVWM**
- **WindowMaker**
- **Enlightenment**

## Desktop Environment

A **Desktop Environment (DE)** is a full suite built on top of the window manager, including:
- file manager
- panels
- system tools
- integrated UI components

Examples:
- **GNOME**
- **KDE Plasma**

---

## Environment Variables

Graphical applications use the `DISPLAY` environment variable to connect to the X server.

Example:
```bash
echo $DISPLAY
```

This tells applications where the X server is running so they can render windows and graphics.

---

# Controls

| Key / Action | Function |
|---|---|
| Mouse Scroll | Zoom in / zoom out |
| ESC | Exit program |
| Window Close Button | Close application |

---

# Compilation

Build the project:

```bash
make
```

make clean
```

make fclean
```

Rebuild project:

```bash
make re
```

---

# Usage

## Mandelbrot

```bash
./fractol mandelbrot
```

## Julia

```bash
./fractol julia
```

Example:

```bash
./fractol julia -0.7 0.27015
```

---

# Technical Concepts

- Complex numbers
- Iterative algorithms
- Coordinate mapping
- Pixel-based rendering
- Event handling
- Real-time rendering loop
- X11 graphical system interaction

---

# Skills Developed

- Low-level graphics programming
- Understanding of Linux GUI architecture (X Window System, X server, window manager)
- Event-driven programming
- Algorithm optimization
- Memory management in C
- Mathematical problem solving
- Performance-focused rendering

---

# Tech Stack

- C
- MiniLibX
- X11
- GCC
- Unix / Linux environment

---

# Author

Fract-ol project completed as part of the 42 Network curriculum.  
Validated with a final score of **100/100**.
