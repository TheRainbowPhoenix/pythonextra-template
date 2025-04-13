# Welcome to PythonExtra for ClassPad

This is a simple starting point for creating Python programs for the ClassPad II (fx-CP400) using **PythonExtra**, a lightweight version of MicroPython built for calculators.


## 🐍 What is Python?

Python is a popular programming language known for its simplicity and readability. It's widely used for teaching, scripting, automation, game development, and much more.

Here’s a simple Python example:

```python
print("Hello, world!")
```

If you're new to Python, no worries—this project is built to help you learn by doing.

> New to Python or the ClassPad?
> Start here:
>
> 👉 [Beginner Guide to PythonExtra](https://classpaddev.github.io/wiki/python/introduction)


## Quick setup

If you haven't already, get the [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python). It would make editing code much easier !

When writing to the calculator, all your Python programs must start with:

```python
import gint
```

This gives you access to the core graphics and input functions available on the calculator.

### What is gint?
`gint` is the main module that powers **drawing**, **keyboard input**, and graphics control in PythonExtra.

You use it for:

- Drawing shapes and pixels (`gint.dpixel`)

- Reacting to key presses (`gint.pollevent()`)

- Controlling the screen update (`gint.dupdate()`)

Here’s a very simple example that draws a **blue rectangle** on screen:

```python
import gint

# Clear the screen with white color
gint.dclear(gint.C_WHITE)

# Draw a filled blue rectangle from (50, 50) to (150, 100)
gint.drect(50, 50, 150, 100, gint.C_BLUE)

# Send drawing to the screen
gint.dupdate()

# Wait for a key press to exit
gint.getkey()
```

> Read more:
>
> 👉 [Beginner Guide to PythonExtra](https://classpaddev.github.io/wiki/python/introduction)
>
> 👉 [gint module reference](https://git.planet-casio.com/Lephenixnoir/PythonExtra/src/branch/main/docs/sh/modgint-en.md)

## 💬 Need Help?

- 🧠 Ask ChatGPT:
    [PythonExtra Helper on ChatGPT](https://chatgpt.com/g/g-67fb8fb50e2c8191a7df1b814ad8fce9-pythonextra-helper)
- 💬 Ask real people on Discord: 
    [SnailMat Server (ClassPad Club)](https://discord.gg/jZQWY9DBKT)

## Project Structure
This repo contains:

- `bounce.py`: A simple boucig logo example (start here!)

- `.typings/` and `.vscode/`: are settings folder for PythonExtra to work on VS Code. Do not delete them.


