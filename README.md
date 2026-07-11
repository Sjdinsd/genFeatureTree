# GenFeatureTree w/ Cmdr
This just adds Cmdr functionality.
Changes: 
- Forces all files under cmdr into their respective folder, no Server/Client seperation
- Added Hook, Type, and Command directory.

## How to use:
1. Add the forked genFeatureTree.js to any path under your project, mine is under tools/.
2. Under src/, add cmdr, cmdr/commands, cmdr/hooks, cmdr/types,
3. Have node and runOnSave inside vsc and use this task under .vscode/tasks.json to auto run on save:
```json
{
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Generate Rojo Project",
            "type": "shell",
            "command": "node tools/genFeatureTree.js",
            "problemMatcher": []
        }
    ]
}
```
<img width="293" height="530" alt="image" src="https://github.com/user-attachments/assets/26f77182-0d90-4534-956e-1440d39af206" />

4. In your startup files, require cmdr on both Server and Client
5. Use Cmdr to your hearts content.

## What this isnt!
- A guide for Cmdr
- You need to know how to use Cmdr

## What this is!
- Allows you to use Cmdr
- ^^^^^
