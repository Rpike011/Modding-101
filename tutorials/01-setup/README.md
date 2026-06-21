# Tutorial 01: Setting Up Your Development Environment

## Objective

Set up all the necessary tools for professional game modding development.

## Prerequisites

- Basic computer literacy
- Administrator access to your computer
- Stable internet connection for downloads

---

## Required Tools Overview

| Tool | Purpose | Required? | Cost |
|------|---------|-----------|------|
| Git | Version control system | ✅ Yes | Free |
| Code Editor/IDE | Write and edit code | ✅ Yes | Free options available |
| Game Framework Tools | Game-specific modding tools | ✅ Yes | Free/Paid |
| Terminal/Bash | Command-line interface | ✅ Yes | Included with Git |
| Mod Management Tools | Organize and test mods | ⚠️ Optional | Free |

---

## Installation Steps

### Step 1: Install Git

**What it is:** Version control system to track changes and collaborate

**Download:** https://git-scm.com/

**Installation:**
1. Visit the link above
2. Click the download button for your operating system
3. Run the installer and follow the prompts
4. **Important:** When asked about "Git Bash," select "Install"

**Verify Installation:**
```bash
git --version
```

You should see something like: `git version 2.40.0`

---

### Step 2: Understanding Bash / Terminal

**What is Bash?**
- A command-line interface (CLI) that lets you type commands instead of clicking
- **Windows:** Called "Git Bash" (installed with Git)
- **Mac/Linux:** Built-in terminal application

**How to Open:**
- **Windows:** Search for "Git Bash" in Start Menu
- **Mac:** Press `Cmd + Space`, type "Terminal", press Enter
- **Linux:** Open Terminal from Applications

**Common Bash Commands:**
```bash
git --version              # Check Git version
cd my-folder              # Change directory (folder)
ls                        # List files (Mac/Linux)
dir                       # List files (Windows)
pwd                       # Show current location
mkdir new-folder          # Create new folder
```

**Why You Need It:**
- Running Git commands
- Navigating your file system
- Running mod tools
- Scripting and automation

---

### Step 3: Choose a Code Editor or IDE

**What it is:** Software to write and edit code files

#### Option A: Visual Studio Code (Recommended for Beginners)

**Download:** https://code.visualstudio.com/

**Why choose it:**
- ✅ Free and lightweight
- ✅ Great Git integration
- ✅ Huge extension library
- ✅ Beginner-friendly

**Installation:**
1. Download for your operating system
2. Run the installer
3. Follow the setup wizard
4. Launch VS Code

**Recommended Extensions:**
- Git Graph
- GitLens
- Code Spell Checker
- Prettier (code formatter)

#### Option B: Sublime Text

**Download:** https://www.sublimetext.com/

**Why choose it:**
- ✅ Very lightweight and fast
- ✅ Minimal learning curve
- ✅ Highly customizable

#### Option C: Notepad++

**Download:** https://notepad-plus-plus.org/

**Why choose it:**
- ✅ Extremely lightweight
- ✅ Good for scripting
- ✅ Simple and straightforward

---

### Step 4: Game-Specific Modding Tools

Depending on which game you're modding, you'll need specific tools:

#### For Skyrim / Fallout Modding

**xEdit (SSEEdit for Skyrim SE)**
- **Download:** https://github.com/TES5Edit/TES5Edit/releases
- **Purpose:** Inspect and edit plugin files (.esp, .esm)
- **Learning:** Essential for serious modders

**Mod Organizer 2**
- **Download:** https://www.modorganizer.org/
- **Purpose:** Organize, install, and manage mods
- **Features:** Virtual file system keeps game folder clean
- **Cost:** Free

**LOOT (Load Order Optimization Tool)**
- **Download:** https://loot.github.io/
- **Purpose:** Automatically sort mod load order
- **Why:** Prevents mod conflicts and crashes
- **Cost:** Free

**Creation Kit**
- **Download:** https://store.steampowered.com/app/1946180/The_Elder_Scrolls_V_Skyrim_Creation_Kit/
- **Purpose:** Official tool for creating content
- **Note:** Available on Steam, free for game owners

**Bethesda Creation Club** (Optional)
- **Website:** https://www.bethesda.net/en/mods
- **Purpose:** Browse and download official content
- **Note:** Some content requires subscription/purchase

#### For Other Games

Search for "[YourGame] modding tools" or check:
- Official game modding wiki
- NexusMods community guides
- Mod.io platform documentation

---

### Step 5: Configure Git

After installation, set up your Git identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

**Verify your configuration:**
```bash
git config --global --list
```

---

## Quick Setup Summary

```bash
# 1. Check Git is installed
git --version

# 2. Configure Git
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# 3. Clone this repository
git clone https://github.com/Rpike011/Modding-101.git
cd Modding-101

# 4. Start learning!
```

---

## Tool Comparison Chart

### Code Editors

| Feature | VS Code | Sublime | Notepad++ |
|---------|---------|---------|-----------|
| Free | ✅ | ⚠️ Trial | ✅ |
| Beginner Friendly | ✅ | ✅ | ✅ |
| Extensions | ✅✅ | ✅ | Limited |
| Git Integration | ✅✅ | ✅ | Basic |
| Performance | Good | Excellent | Excellent |

### Mod Management Tools

| Tool | Purpose | Free | Difficulty |
|------|---------|------|------------|
| Mod Organizer 2 | Mod management & virtual file system | ✅ | Medium |
| LOOT | Automatic load order sorting | ✅ | Easy |
| xEdit | Plugin inspection & editing | ✅ | Hard |
| Creation Kit | Official content creation | ✅ | Hard |

---

## Troubleshooting

### "git command not found"
- **Solution:** Git not installed or not in system PATH
- **Fix:** Reinstall Git and restart terminal

### "Permission Denied" errors
- **Solution:** Run terminal as Administrator (Windows) or use `sudo` (Mac/Linux)

### Editor won't open files
- **Solution:** Check file permissions or run as administrator

### Mod tools won't launch
- **Solution:** Install required .NET Framework or Visual C++ Redistributables
- **Download:** https://dotnet.microsoft.com/

---

## Next Steps

1. ✅ Install all required tools
2. ✅ Open Terminal/Git Bash and verify installations
3. ✅ Configure Git with your name and email
4. ➡️ Proceed to [Tutorial 02: Creating Your First Mod](../02-first-mod/)

---

## Useful Resources

- [Git Documentation](https://git-scm.com/doc)
- [VS Code Documentation](https://code.visualstudio.com/docs)
- [Official Game Modding Wikis](https://en.uesp.net/wiki/) (for TES games)
- [NexusMods Community Guides](https://www.nexusmods.com/)
- [Mod.io Documentation](https://mod.io/developers)

---

## Questions?

Having trouble with setup? Check [CONTRIBUTING.md](../../CONTRIBUTING.md) to ask for help!
