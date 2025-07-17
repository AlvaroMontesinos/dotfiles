# Tmux Configuration Manual

## 🎯 Prefix Key
- `Ctrl+a` - Main prefix key (replaces default Ctrl+b)

---

## 🪟 Window Management

### **No-Prefix Window Controls (Ultra Fast)**
| Key | Action |
|-----|--------|
| `Alt+1-9,0` | Switch to window 1-10 instantly |
| `Alt+n` | Create new window in current directory |
| `Alt+q` | Kill current window |
| `Alt+r` | Rename current window |

### **Prefix-Based Window Controls**
| Key | Action |
|-----|--------|
| `Ctrl+a a` | Switch to last window |
| `Ctrl+a c` | Create new window in current directory |
| `Ctrl+a n` | Next window |
| `Ctrl+a p` | Previous window |
| `Ctrl+a w` | Choose window interactively |
| `Ctrl+a ,` | Rename current window |
| `Ctrl+a '` | Select window by index prompt |
| `Ctrl+a X` | Kill current window |
| `Ctrl+a 1-9,0` | Switch to window by number |

### **Window Navigation (No Prefix)**
| Key | Action |
|-----|--------|
| `Ctrl+PageUp` | Previous window |
| `Ctrl+PageDown` | Next window |

### **Window Swapping**
| Key | Action |
|-----|--------|
| `Ctrl+a Ctrl+p` | Move window left |
| `Ctrl+a Ctrl+n` | Move window right |

---

## 📋 Pane Management

### **No-Prefix Pane Controls (Ultra Fast)**
| Key | Action |
|-----|--------|
| `Alt+h` | Navigate to left pane |
| `Alt+j` | Navigate to down pane |
| `Alt+k` | Navigate to up pane |
| `Alt+l` | Navigate to right pane |
| `Alt+v` | Split horizontally (side-by-side) |
| `Alt+s` | Split vertically (top-bottom) |
| `Alt+x` | Kill current pane |
| `Alt+z` | Toggle pane zoom (maximize/restore) |

### **Prefix-Based Pane Navigation**
| Key | Action |
|-----|--------|
| `Ctrl+a h` | Navigate to left pane |
| `Ctrl+a j` | Navigate to down pane |
| `Ctrl+a k` | Navigate to up pane |
| `Ctrl+a l` | Navigate to right pane |
| `Ctrl+a q` | Display pane numbers |
| `Ctrl+a z` | Toggle pane zoom |
| `Ctrl+a Z` | Toggle pane zoom (alternative) |
| `Ctrl+a !` | Break pane into new window |
| `Ctrl+a @` | Join pane horizontally from last window |
| `Ctrl+a t` | Mark current pane |
| `Ctrl+a T` | Swap with marked pane |

### **Pane Splitting**
| Key | Action |
|-----|--------|
| `Ctrl+a \|` | Split horizontally (side-by-side) |
| `Ctrl+a \` | Split horizontally (side-by-side) |
| `Ctrl+a v` | Split horizontally (side-by-side) |
| `Ctrl+a -` | Split vertically (top-bottom) |
| `Ctrl+a _` | Split vertically (top-bottom) |
| `Ctrl+a s` | Split vertically (top-bottom) |

### **Pane Resizing**
| Key | Action |
|-----|--------|
| `Ctrl+a H` | Fine resize left (1 cell) |
| `Ctrl+a J` | Fine resize down (1 cell) |
| `Ctrl+a K` | Fine resize up (1 cell) |
| `Ctrl+a L` | Fine resize right (1 cell) |
| `Ctrl+a ←` | Resize left (5 cells, repeatable) |
| `Ctrl+a ↓` | Resize down (5 cells, repeatable) |
| `Ctrl+a ↑` | Resize up (5 cells, repeatable) |
| `Ctrl+a →` | Resize right (5 cells, repeatable) |

### **Pane Management**
| Key | Action |
|-----|--------|
| `Ctrl+a x` | Kill current pane |
| `Ctrl+a X` | Kill current window |

---

## 🎛️ Layout Management
| Key | Action |
|-----|--------|
| `Ctrl+a Space` | Cycle through preset layouts |
| `Ctrl+a Alt+1` | Even horizontal layout |
| `Ctrl+a Alt+2` | Even vertical layout |
| `Ctrl+a Alt+3` | Main horizontal layout |
| `Ctrl+a Alt+4` | Main vertical layout |
| `Ctrl+a Alt+5` | Tiled layout |

---

## 📋 Copy Mode & Search
| Key | Action |
|-----|--------|
| `Ctrl+a f` | Enter copy mode and search forward |
| `Ctrl+a F` | Enter copy mode and search backward |
| Mouse selection | Automatically copies to system clipboard |

---

## ⚡ Productivity Tools

### **Clear Commands**
| Key | Action |
|-----|--------|
| `Ctrl+a Ctrl+k` | Send `clear` command to terminal |
| `Ctrl+a Ctrl+y` | Clear tmux history buffer |
| `Ctrl+a Ctrl+l` | Clear screen and history |

### **System Operations**
| Key | Action |
|-----|--------|
| `Ctrl+a :` | Open command prompt |
| `Ctrl+a r` | Reload configuration file (with confirmation) |
| `Ctrl+a R` | Respawn dead pane |
| `Ctrl+a Ctrl+r` | Respawn entire window |

### **Synchronization & Monitoring**
| Key | Action |
|-----|--------|
| `Ctrl+a e` | Enable pane synchronization |
| `Ctrl+a E` | Disable pane synchronization |
| `Ctrl+a y` | Toggle pane synchronization |
| `Ctrl+a A` | Monitor window activity |
| `Ctrl+a M` | Monitor silence (30 seconds) |

---

## 🔍 Enhanced Search & Text Extraction

### **Plugin-Based Features**
| Key | Action |
|-----|--------|
| `Ctrl+a Tab` | **Extrakto** - Extract text/URLs/paths from output |
| `Ctrl+a o` | **FPP** - Facebook Path Picker for file selection |
| `Ctrl+a u` | **URLView** - View and open URLs from output |

---

## 🖱️ Mouse Support
- ✅ Full mouse support enabled
- ✅ Click to select panes
- ✅ Drag to resize panes
- ✅ Scroll to navigate history
- ✅ Mouse selection auto-copies to clipboard
- ❌ Right-click menu disabled

---

## 📊 System Monitoring & Status Bar

### **Status Bar Information**
- **Left**: Session name
- **Center**: Window list with activity indicators
- **Right**: CPU usage, battery status, time (HH:MM), date (DD.MM.YYYY)

### **CPU & Battery Icons**
- **CPU**: `=` (low), `≡` (medium), `≣` (high)
- **Battery**: `♥` (full), `♡` (empty)

---

## 🔌 Installed Plugins

### **Core Plugins**
- **tpm** - Tmux Plugin Manager
- **tmux-sensible** - Sensible default settings
- **tmux-resurrect** - Save/restore sessions manually
- **tmux-continuum** - Auto-save sessions every 15 minutes
- **tmux-yank** - Enhanced clipboard operations
- **tmux-open** - Open files and URLs from tmux

### **Productivity Plugins**
- **tmux-pain-control** - Better pane management
- **tmux-copycat** - Enhanced search in copy mode
- **tmux-logging** - Log pane outputs to `~/.tmux/logs`
- **tmux-sessionist** - Advanced session management
- **tmux-fpp** - Facebook Path Picker integration
- **tmux-urlview** - URL extraction and opening
- **tmux-cpu** - CPU usage display
- **tmux-battery** - Battery status display
- **extrakto** - Extract and copy text/URLs/paths

### **Plugin Management**
| Key | Action |
|-----|--------|
| `Ctrl+a I` | Install/update plugins |
| `Ctrl+a U` | Update plugins |
| `Ctrl+a Alt+u` | Uninstall plugins not in config |

---

## ⚙️ System Settings & Performance

### **Performance Optimizations**
- 📊 100,000 lines of scrollback history
- ⚡ No escape time delay (0ms)
- 🔄 5-second status bar updates
- 📈 Aggressive resize for multiple clients
- 💾 50 buffer limit for memory efficiency
- 📝 Command history saved to `~/.tmux_history`

### **Visual & Terminal Features**
- 🎨 256-color terminal support with true color (RGB)
- 📐 Underline styles support
- 📍 Status bar positioned at top
- 🎨 Iceberg color scheme (dark blue/gray palette)
- 📊 Activity monitoring with visual indicators
- 🔲 Simplified pane borders
- 🔇 All bells and visual notifications disabled

### **Behavior Settings**
- 🔢 Windows and panes start at index 1
- 🔄 Automatic window renumbering when deleted
- 📁 Current directory shown as window title
- ⌨️ Vim keybindings for navigation and copy mode
- ⌨️ Emacs keybindings for command prompt
- 🖱️ Mouse support fully enabled
- 🎯 Focus events enabled for editor integration
- ⌨️ Xterm keys enabled for better terminal compatibility

### **Shell Integration**
- 🐚 Default shell: **zsh** on both macOS and Linux
- 📝 Better word separators for text selection: ` @"=()[]{}:,.`
- 📋 External clipboard integration with auto-detection
- 🐧 Wayland (`wl-copy`) and X11 (`xclip`) support

---

## 🔧 Advanced Features

### **Session Persistence**
- 💾 Auto-save sessions every 15 minutes
- 🔄 Automatic session restoration on tmux start
- 📝 Vim/Neovim session restoration
- 📋 Pane content capture in saved sessions
- 🔄 Process restoration for: `ssh`, `mysql`, `psql`
- 🚀 Boot-time session restoration

### **Logging & Monitoring**
- 📝 All session output logged to `~/.tmux/logs`
- 📊 Activity and silence monitoring per window
- 🎨 Visual activity indicators in status bar
- 💻 System resource monitoring (CPU, battery)

---

## 🎨 Color Scheme (Iceberg Theme)
- **Foreground**: `#c6c8d1`
- **Medium Background**: `#4c566a`
- **Dark Background**: `#3b4252`
- **Very Dark Background**: `#2e3440`
- 🔴 Activity highlighting in red/yellow
- 🎨 Consistent color scheme across all elements

---

## 🚀 Quick Start Tips

### **Essential No-Prefix Keys**
- `Alt+h/j/k/l` - Navigate panes instantly
- `Alt+1-9` - Switch windows instantly
- `Alt+v/s` - Split panes instantly
- `Alt+n` - New window instantly

### **Most Used Prefix Keys**
- `Ctrl+a r` - Reload config
- `Ctrl+a z` - Zoom pane
- `Ctrl+a :` - Command prompt
- `Ctrl+a I` - Install plugins

### **Installation**
1. Install plugins: `Ctrl+a I`
2. Create log directory: `mkdir -p ~/.tmux/logs`
3. Reload config: `Ctrl+a r`

---

*This configuration provides lightning-fast navigation, comprehensive development tools, advanced session management, and extensive customization for maximum productivity in terminal environments.*