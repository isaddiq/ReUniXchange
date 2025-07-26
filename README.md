# ReUniXchange: BIM to Unity Metadata Export Plugin for Revit

ReUniXchange is a custom Autodesk Revit plugin designed to facilitate seamless export of Building Information Modeling (BIM) data, including geometry and semantic metadata, for use in Unity-based XR (AR/VR/MR) environments. This tool enables bidirectional data flow by converting Revit models into Unity-compatible formats and preserving BIM semantics for use in immersive design review, construction simulation, and facility management.

---

## ✨ Key Features

- Export Revit 3D geometry to **OBJ format** with material and texture information
- Export BIM metadata (element properties) to **CSV format**
- Assign **Modular Group IDs** to support modular construction workflows
- Automatically link geometry and metadata using **Element IDs**
- Designed for downstream integration with the **ReUniXchange Unity Package**

---

## 🛠️ Requirements

- **Autodesk Revit 2024, 2025, or 2026 (During installation change the directory folder to specific version of Revit) ** 
- .NET Framework 4.8
- Visual Studio (for development and compilation)
- Admin access to install Revit plugins

---

## 📁 Exported Files

When using ReUniXchange, the following files are generated for use in Unity:

| File | Description |
|------|-------------|
| `.obj` | Geometry file exported from current Revit 3D view |
| `.mtl` | Material file accompanying the OBJ geometry |
| `.csv` | Metadata file containing element properties |
| `SharedParams.txt` | Optional shared parameter file for Modular Group ID |

---

## 🔧 Plugin Tools (Ribbon Tab: ReUniXchange)

1. **Assign Modular Parameter**  
   Adds a shared parameter `Modular_Group_Id` to elements within Revit groups

2. **Export Metadata**  
   Extracts user-selected element parameters into a `.csv` file

3. **Export Material**  
   Exports material definitions and colors used in the model

4. **Export OBJ**  
   Converts the current 3D view into an `.obj` file with geometry and textures

5. **Import XML**  
   [Optional] Allows re-import of processed data from Unity pipeline

6. **About Me**  
   Displays plugin version, credits, and links to documentation

---

## 🚀 How to Use

1. Open your Revit model and navigate to a 3D view with visible elements
2. Click **Assign Modular Parameter** if your project includes grouped modular units
3. Select **Export Metadata** and choose parameters to include in the CSV
4. Use **Export OBJ** to generate the 3D model for Unity
5. Transfer `.obj`, `.mtl`, and `.csv` to Unity and import using the ReUniXchange Unity package

---

## 📦 Integration with Unity

Use the **ReUniXchange Unity Package** (available separately) to:
- Parse `.obj` geometry
- Link metadata from `.csv`
- Automatically build BIM hierarchy and metadata viewers in Unity
- Deploy to XR platforms (Meta Quest, PC VR, Android AR)

---

## 📚 Documentation

- [User Guide](#) (Coming Soon)
- [Unity Integration Wiki](#) (Coming Soon)
- [Issue Tracker](https://github.com/YourUsername/ReUniXchange/issues)

---

## 📄 License

MIT License. See [LICENSE](LICENSE) for details.

---

## 👤 Author

Saddiq Ur Rehman  
PhD Researcher, Kyung Hee University  

---

## 💬 Feedback & Contributions

Feedback, suggestions, and contributions are welcome! Please open an issue or pull request if you'd like to collaborate.

---

## 🎥 Demo Video

[![ReUniXchange Demo](https://img.youtube.com/vi/CQp8Uhdefsk/maxresdefault.jpg)](https://www.youtube.com/watch?v=CQp8Uhdefsk&t=56s)

*Click the image above to watch the demonstration*
