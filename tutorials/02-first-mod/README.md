# Tutorial 02: Creating Your First Mod

## Objective

Create your first simple mod and understand the basic structure.

## Prerequisites

- Completed [Tutorial 01: Setup](../01-setup/)
- Git installed and configured
- Code editor ready

## What You'll Learn

- Basic mod file structure
- How to create a simple mod
- How to use Git to version control your mod

## Getting Started

### Step 1: Create Your Mod Directory

```bash
cd Modding-101/mods
mkdir my-first-mod
cd my-first-mod
```

### Step 2: Initialize Git

```bash
git init
```

### Step 3: Create Basic Mod Files

Create the following structure:

```
my-first-mod/
├── README.md
├── mod.json
└── src/
    └── main.js
```

### Step 4: Add Content

**mod.json** - Mod metadata:
```json
{
  "name": "My First Mod",
  "version": "1.0.0",
  "description": "A simple beginner mod",
  "author": "Your Name",
  "main": "src/main.js"
}
```

**src/main.js** - Main mod file:
```javascript
// My First Mod
console.log("My first mod is loaded!");

// Add your mod logic here
export function onLoad() {
  console.log("Mod initialized!");
}
```

### Step 5: Commit Your Changes

```bash
git add .
git commit -m "Initial mod structure"
```

## Understanding Git Basics

| Command | Purpose |
|---------|---------|
| `git add .` | Stage all changes |
| `git commit -m "message"` | Save changes with description |
| `git log` | View commit history |
| `git status` | See current changes |

## Next Steps

- Explore the mod framework documentation
- Add more features to your mod
- Learn about version control workflows

## Troubleshooting

### Changes not committed
- Use `git status` to see what's staged
- Make sure you `git add` before `git commit`

## Next Tutorial

Proceed to [Tutorial 03: Advanced Concepts](../03-advanced/)
