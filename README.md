# 🚀 NguyenHoang BIM Tools  
### Revit 2024 Productivity Toolkit for Structural & BIM Workflows

---

## 📌 Overview
**NguyenHoang BIM Tools** is a powerful Revit add-in designed to automate and streamline structural BIM workflows, with a strong focus on **rebar detailing, calculation, and batch export**.

Built for real-world production environments, this tool helps reduce manual work, improve accuracy, and standardize outputs across projects.

---

## ⚙️ Supported Version
- ✅ Autodesk Revit **2024**
- ⚠️ Other versions are not guaranteed (separate build required)

---

## ✨ Key Features

### 🔩 Rebar Management
- Explode Rebar Sets → Single FreeForm Rebars  
- Group Single Rebars → FreeForm Set  
- Preserve:
  - Partition  
  - Schedule Mark  
  - Rebar Style  
  - Hook orientation & angles (90°, 135°, etc.)  
- Smart handling of:
  - Hook synchronization  
  - Multi-planar curves  
  - Excluded bars  

---

### 📊 Rebar Calculation System
- Fully automated rebar calculation pipeline:
  - Classify by shape (M_SP and others)
  - Lap splice length processing
  - Average length calculation
  - Quantity detection & classification
  - Total length calculation
  - Case classification

- Auto update parameters:
  - Length
  - Quantity
  - Weight

- Smart error handling per row (UI feedback)

---

### 📋 Schedule Automation
- Auto-create **Rebar Schedule**
- Apply standardized formatting:
  - Column naming
  - Units (mm, kg/m)
  - Sorting & grouping
  - Grand total

- Copy schedules directly from template `.rte`

---

### 🗑️ Delete Multiple Tool
- Batch delete:
  - Shared Parameters
  - Filters
  - Materials
  - View Templates

- UI with:
  - Checkbox selection
  - Status message per item
  - Error feedback

---

### 🎨 Visualization Tools
- Filter-based color highlighting
- Control element visibility
- Improve model readability for QA/QC

---

### 📤 IFC Batch Export
- Export multiple Revit files at once
- Auto-detect best 3D view:
  - `{3D}`
  - `3D CDE`
  - `3D NAVISWORKS (KHÔNG CỐT THÉP)`

- Use JSON-based IFC settings
- Progress tracking with per-file status
- Fully automated export workflow

---

### 📦 3D CAD (DWG) Export *(in development / extended)*
- Export DWG from 3D views
- Auto-transfer export settings from template if missing
- Consistent output across projects

---

### 🔄 Smart Update System
- No need to reinstall manually
- Tool uses **GitHub Releases** as cloud source
- Always fetch latest version package
- Lightweight bootstrap updater

---

### 🎯 UI/UX Highlights
- Modeless WPF UI (work while tool is open)
- Progress bar with step-by-step status
- ListView with:
  - Checkbox selection
  - Status messages
  - Color-coded feedback

---

## 📦 Installation Guide

### 🔧 First-time Setup

1. Download the latest **Setup / Bootstrapper**
2. Run the installer

The installer will:
- Create folder:
- Download latest version from GitHub
- Install all required files (DLL, JSON, RTE…)
- Create Revit add-in file at: %AppData%\Autodesk\Revit\Addins\2024


---

### 🔁 Update to Latest Version

Simply run the **same installer again**

✔ It will:
- Pull latest release from GitHub  
- Replace old files automatically  
- Keep your setup up-to-date  

⚠️ Make sure **Revit is closed** before updating

---

## 📁 Installation Structure
C:\NguyenHoangTools
NguyenHoang.Tools.dll
Google.Apis.dll
HL_EXPORT_IFC_SETTING.json
HOANGLONG_TEMPLATE_RVT24.rte
...

%AppData%\Autodesk\Revit\Addins\2024
NguyenHoang.Tools.addin


---

## 🧠 Design Philosophy
- ✔ Automation over manual work  
- ✔ Consistency across projects  
- ✔ Production-ready workflows  
- ✔ Clean UI + clear feedback  
- ✔ Easy deployment & update  

---

## ⚠️ Notes
- Tool is optimized for **structural BIM workflows**
- Requires correct project setup for best results (parameters, templates, etc.)
- Some features depend on template files included in installation

---

## 📌 Future Improvements
- Auto-update inside Revit UI  
- More export formats (DWG, Navisworks)  
- Advanced rebar grouping logic  
- Performance optimization for large models  

---

## 👨‍💻 Author
**Nguyen Hoang**  
BIM Developer | Revit API | Structural BIM  

---

## ⭐ Support
If you find this tool useful, feel free to:
- ⭐ Star the repository
- Share with your team
- Suggest improvements

---

## 🚀 Versioning
All versions are managed via **GitHub Releases**  
→ Always download or update to the latest version for best performance
