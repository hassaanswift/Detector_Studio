# 🎯 Detector Studio — Fast Annotation Tool

A high-performance, keyboard-driven annotation tool for object detection (YOLO format). Designed to make your annotation workflow faster, smoother, and completely organized.

## ✨ Key Features

- **Smart `.txt` Lifecycle**: Automatically creates a YOLO `.txt` file when you draw your first box. If you delete all boxes, it automatically deletes the empty `.txt` file.
- **Keyboard-First Workflow**: Specially designed to minimize mouse usage and maximize speed.
- **`R` Key Magic**: Instantly copy all annotations from the previous image to the current one.
- **Right-Click Delete**: Just right-click on any bounding box to delete it instantly.
- **Dynamic Class Panel**: Only shows the classes you add. `1-9` shortcuts automatically map to your available classes.
- **Modern Neon UI**: A beautiful, deep-dark theme with neon green accents that reduces eye strain during long hours of annotation.
- **Undo / Redo**: Multi-level undo/redo stack to fix mistakes quickly.
- **Auto-Next Mode**: Optionally move to the next image automatically after drawing a box.
- **Jump to Unlabeled**: `Ctrl+Shift+N` takes you straight to the next image that doesn't have a `.txt` file yet.

## ⌨️ Shortcut Guide

| Key / Shortcut | Action |
| :--- | :--- |
| **Mouse Left-Drag** | Draw a bounding box |
| **Mouse Right-Click** | Delete hovered box |
| **R** | Copy annotations from previous image |
| **A / Left Arrow** | Previous Image |
| **D / Right Arrow** | Next Image |
| **N** | Mark current image as "No Object" & go Next |
| **1 - 9** | Assign class ID to selected box |
| **Delete** | Delete selected box |
| **Ctrl + Z / Ctrl + Y** | Undo / Redo |
| **Ctrl + D** | Duplicate selected box |
| **Ctrl + Shift + A** | Toggle Auto-Next mode |
| **Ctrl + Shift + N** | Jump to next unlabeled image |
| **F** | Fit image to window |
| **Mouse Wheel** | Zoom In / Out (zooms to cursor) |
| **Middle Mouse Drag** | Pan image |

## 🚀 How to Use

1. Download the `Detector.exe` from the Assets section below.
2. Double-click to open the application (No Python installation required).
3. Click on **"Select Image Folder"** and choose your dataset folder.
4. Add your classes in the right panel (this will create a `classes.txt` file in the app folder).
5. Start annotating! Your progress is auto-saved.

## 📦 Build from Source (For Developers)

If you want to run it from the source code:
```bash
git clone https://github.com/hassaanswift/Detector_Studio.git
cd Detector_Studio
python -m venv venv
venv\Scripts\activate
pip install PySide6
python main.py
