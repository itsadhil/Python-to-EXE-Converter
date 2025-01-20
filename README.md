# Python to EXE Converter

This Python program allows you to convert any Python script (`.py`) into a standalone executable (`.exe`) file. The program provides a modern, user-friendly interface to select the Python script, choose the destination folder, and convert the script into an executable.

## Features

- **Easy-to-Use Interface**: A clean and modern UI to select the Python file and destination folder.
- **Conversion Progress**: A loading progress bar that shows the status during the conversion process.
- **Destination Selection**: Choose the folder where the generated `.exe` will be saved.
- **No Command Line Required**: Convert Python scripts to `.exe` without needing to use the command line.

## Requirements

- Python 3.x
- Tkinter (for the GUI)
- PyInstaller (for converting `.py` files to `.exe`)

## Installation

1. **Install Python**: Ensure you have Python 3.x installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

2. **Install Required Libraries**:
   To install the required libraries (`tkinter` and `PyInstaller`), you can run:

   ```bash
   pip install pyinstaller
   ```

   `tkinter` is included by default with Python, so no need to install it separately.

3. **Download the Program**:
   Download the `pytoexe.py` script to your local machine.

## Usage

1. Run the `pytoexe.py` script.

   ```bash
   python pytoexe.py
   ```

2. A window will appear with the following options:
   - **Select Python File**: Click this button to select the Python script (`.py`) you want to convert to `.exe`.
   - **Select Destination Folder**: Click this button to choose the folder where the `.exe` will be saved.
   - **Convert to EXE**: After selecting the file and destination folder, click this button to start the conversion. A progress bar will appear to show the conversion status.

3. Once the conversion is complete, the executable (`.exe`) will be available in the selected destination folder.

## How It Works

This program uses [PyInstaller](https://www.pyinstaller.org/) to convert the Python file to an executable. PyInstaller bundles the Python script, all its dependencies, and the Python interpreter into a single `.exe` file.

### Conversion Command
The program uses the following command to convert the Python script:

```bash
pyinstaller --onefile --noconsole <path_to_python_file>
```

- `--onefile`: Packages everything into a single executable.
- `--noconsole`: Disables the console window for GUI-based scripts.

## License

This project is licensed under the MIT License.

```

This `README.md` provides clear instructions on how to set up, install, and use your Python to EXE converter tool. You can customize or add more information as necessary for your project.
