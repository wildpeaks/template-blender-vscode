# Template: Blender script


## Setup

Python:
1. Install **Python 3** from https://www.python.org/ and enable `Add to PATH` option during install.
2. Disable the placeholder aliases `python.exe` and `python3.exe` in `Start Menu` → `Manage app execution aliases`

VSCode:
1. Install **VSCode** from https://code.visualstudio.com/.
2. Open this folder in VSCode: it will prompt you to install recommended extensions (the list is defined in `/.vscode/extensions.json`).
3. When you have a `.py` file open in VSCode, click `Select Interpreter` (in the status bar at the bottom) to pick the Python version you just installed.
4. Open a Terminal in VSCode and run: `pip install fake-bpy-module-3.2` (to match Blender 3.2.x)
5. Restart VSCode

At this stage, you should have Intellisense for simple scripts:
```py
import math
print(math.pi)
```
and Blender scripts:
```py
import bpy
bpy.ops.mesh.primitive_monkey_add()
```

## Run in Blender

1. In Blender `Scripting` workspace, in the text editor, click `Open` and locate your `.py` file. This will open it in Blender's text editor.
2. Click the triangle button `Run Script` to execute it once.
3. From now on, you can edit in VSCode but it won't show the changed script in Blender's text editor unless you click the red `Resolve conflict` → `Reload from disk` button.

You can skip clicking Reload and click only Run using a second scrip, see template `External Script Stub` and https://docs.blender.org/api/current/info_tips_and_tricks.html#executing-external-scripts.
