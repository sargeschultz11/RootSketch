# 🌳 RootSketch

RootSketch is a lightweight and straightforward tool that generates a text-based visualization of the folder and file structure of your project. Whether you're a developer, project maintainer, or just organizing files, RootSketch creates an organized, hierarchical representation of your project's directory, saved as a text file for easy reference.

## ✨ Features

- **Tree-Like Visualization:** Outputs directories and files in a clean, tree-like format with proper indentation and symbols (`├──`, `└──`, etc.).
- **Pre-Packaged Executable:** No need to install Python! Download the ready-to-use `.exe` and run it instantly.
- **Customizable:** Easily exclude specific directories and files by modifying the `ignore_list` in the Python script.
- **Quick and Efficient:** Generates a full project structure in seconds.
- **Portable:** A single executable or script for portable use.

## 📋 Example Output

Here’s an example of the output generated by RootSketch:

```
MyProject/
├── assets/
│   ├── fonts/
│   │   └── Rubik-Regular.ttf
│   ├── icon.ico
│   └── logo.png
├── components/
│   ├── backup_manager.py
│   ├── database_manager.py
│   ├── logger.py
│   └── scheduler.py
├── ui/
│   ├── add_task_dialog.py
│   └── edit_task_dialog.py
├── .gitignore
├── LICENSE
├── README.md
├── main.py
├── pybut_tasks.db
└── requirements.txt
```

## 🚀 Getting Started

### 📥 Download the Executable

To make things easier, we've provided a pre-packaged `.exe` file. You can download it directly from the [Releases](https://github.com/sargeschultz11/RootSketch/releases) section of this repository.

1. Go to the [Releases](https://github.com/sargeschultz11/RootSketch/releases) page.
2. Download the latest `RootSketch.exe`.
3. Place the `.exe` in the root directory of your project.
4. Run it by double-clicking or via the terminal.

### 🐍 Using the Python Script (Optional)

If you'd prefer to use the Python script:

1. Clone the repository:
   ```bash
   git clone https://github.com/sargeschultz11/RootSketch.git
   cd RootSketch
   ```

2. Run the script:
   ```bash
   python RootSketch.py
   ```

3. Open the generated `project_structure.txt` file in the same directory to view your project's folder structure.

## 🛠 Customization

If you want to customize RootSketch:

- **Excluding Items:** Update the `ignore_list` in the script to add or remove directories/files from the output:
  ```python
  ignore_list = {".git", "__pycache__", "RootSketch.py", "project_structure.txt", "RootSketch.exe"}
  ```

- **Formatting:** Modify the indentation or tree symbols in the `write_structure` function.

## 🧑‍💻 Self-Packing

If you want to package the script into an `.exe` yourself:

1. Install PyInstaller:
   ```bash
   pip install pyinstaller
   ```

2. Package the script:
   ```bash
   pyinstaller --noconsole --onefile src/RootSketch.py
   ```

3. Find the executable in the `dist/` folder.

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

Thanks to the Python Software Foundation.

Thank you for checking out RootSketch! If you find this tool helpful, feel free to star the repository and share it with others.

---

Enjoy your trees! 🌳
