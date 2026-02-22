# <img src="CheckFEM_logo.png" width="48" height="48" align="center">&nbsp; CheckFEM

**CheckFEM** is a specialized quality control tool for **Finite Element (FE) models**. It streamlines the validation process by parsing raw model data into a structured database, allowing for advanced automated checks and 3D visualization.

## 🚀 Key Features

*   **Multi-Format ASCII Parsers:** Specifically engineered for:
    *   **Ansys** (`.dat`, `.inp`)
    *   **Samcef** (`.dat`)
    *   *Status:* Ongoing development. While core commands are supported, full card coverage is being expanded.
    *   *Roadmap:* Future updates will include support for **Nastran** (`.bdf`), **Abaqus** (`.inp`), and other major FEA formats.
*   **Structured Data Storage:** 
    *   Parses model commands (cards) automatically.
    *   Stores all entities (nodes, elements, properties, loads) into a local **H2 Database**.
*   **Custom Scripting:** 
    *   Users can write **Java** scripts to query the database.
    *   Perform custom calculations and extract specific model attributes.
*   **3D Visualization:** 
    *   High-performance 3D interface powered by **VTK**.
    *   Visually inspect model quality, connectivity, and results.

## 📦 Getting Started (Demo)

The release `.zip` package is ready-to-use and includes:
*   📂 **Demo Models:** Sample files for both Ansys and Samcef to test the parser.
*   ✅ **Checklists:** Pre-configured demo scripts to show how to automate model verification.

## ⚙️ How It Works

1.  **Import:** Load your Ansys or Samcef file into CheckFEM.
2.  **Process:** The internal parser identifies supported cards and populates the local H2 engine.
3.  **Analyze:** Run quality scripts (using the provided demo checklists).
4.  **Visualize:** Display identified issues in the 3D viewer for manual review.

## 🛠 Tech Stack

*   **Core:** Java (OpenJDK 8)
*   **Database:** [H2 Database Engine](https://h2database.com)
*   **Graphics:** [VTK (Visualization Toolkit)](https://vtk.org)
*   **UI Extensions:** SwingX
*   **Parsing Tools:** JavaCC & JTB

## ⚖️ Licensing

This software is currently in **Alpha version**.
*   Provided "as-is" for evaluation purposes.
*   Usage is governed by a free 1-year license (see `LICENSE` for details).
*   Third-party component credits are listed in the `NOTICE` file.
