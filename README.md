# VisGuithon — Data Visualization Dashboard

A multi-chart data visualization dashboard built with **pyimgui** (Dear ImGui) + GLFW + OpenGL.  
Architecture inspired by [ochisrj/VisGuithon](https://github.com/ochisrj/VisGuithon).

## Features

FUCK YOU IT NOT FINISH 

## Setup

```bash
pip install -r requirements.txt
python main.py
```

fix bug

## Usage

- **Dashboard tab** — auto-populated with live stats + first CSV columns
- **CSV Data tab** — pick X/Y columns and chart type via sidebar
- **Live Stats tab** — real-time system gauges, per-core bars, network/disk history
- **File → Load CSV/Excel** — type the file path in the dialog
- **File → Load Sample Data** — regenerates `data/sample.csv` (60 rows of business metrics)

## Keyboard Shortcuts

| Key | Action |
|---|---|
| Ctrl+O | Open file dialog |
| Ctrl+D | Load sample data |
| Ctrl+Q | Quit |
