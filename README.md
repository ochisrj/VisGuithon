# VisGuithon - Python Text Editor (pyimgui)

A feature-rich text editor built with Python + pyimgui (Dear ImGui).

## Features
- 📝 Multi-tab text editor
- 🎨 Syntax highlighting (Python keywords)
- 💻 Built-in local terminal (run files like PowerShell)
- ⚙️ Preferences panel (theme, font, scale)
- 📂 File open/save dialogs

## Project Structure

```
VisGuithon/
├── main.py                  # Entry point
├── config.py                # App-wide constants & defaults
├── requirements.txt         # Dependencies
│
├── core/
│   ├── __init__.py
│   ├── app.py               # Main App class (window loop, layout)
│   ├── editor.py            # Text editor logic (tabs, buffer, cursor)
│   ├── file_manager.py      # Open / Save / New file I/O
│   ├── highlighter.py       # Syntax highlighting engine
│   └── terminal.py          # Embedded terminal (subprocess runner)
│
├── ui/
│   ├── __init__.py
│   ├── menu_bar.py          # Top menu bar (File, Edit, View, Run)
│   ├── editor_panel.py      # Editor panel renderer
│   ├── terminal_panel.py    # Terminal panel renderer
│   ├── preferences.py       # Preferences popup window
│   └── status_bar.py        # Bottom status bar (line/col, encoding)
│
├── themes/
│   ├── __init__.py
│   ├── theme_manager.py     # Load & apply imgui color themes
│   ├── dark.py              # Dark theme colors
│   ├── light.py             # Light theme colors
│   └── monokai.py           # Monokai theme colors
│
└── utils/
    ├── __init__.py
    ├── settings.py          # Load/save user preferences (JSON)
    └── helpers.py           # Misc utilities (path formatting, etc.)
```

## Setup

```bash
pip install pyimgui[glfw] pyopengl
python main.py
```

## Keyboard Shortcuts
| Shortcut       | Action          |
|----------------|-----------------|
| Ctrl+N         | New file        |
| Ctrl+O         | Open file       |
| Ctrl+S         | Save file       |
| Ctrl+Shift+S   | Save as         |
| Ctrl+`         | Toggle terminal |
| Ctrl+,         | Preferences     |
| F5             | Run current file|
