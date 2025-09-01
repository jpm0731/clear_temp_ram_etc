# Clear Temp RAM ETC

This project provides a Python script and executable for cleaning temporary files, internet cache, history, prefetch files, and emptying the Recycle Bin on Windows systems. It features a minimalistic GUI with a "Clean it" button and real-time log output.

## Features

- Deletes temporary user and system files (%TEMP%)
- Clears temporary internet files and history
- Deletes prefetch files
- Empties the Recycle Bin for drives C, D, and E
- Minimalistic GUI with:
  - Full-width "Clean it" button
  - Real-time log display of cleaned items
  - Red "Close" button
  - No window border or control buttons (minimize, maximize, close)
- Packaged as a standalone executable with administrator privileges
- Custom icon (`data-cleaning.ico`)

## Usage

### Running the Python Script

1. Ensure you have Python 3 installed.
2. Install dependencies:
   ```
   pip install customtkinter
   ```
3. Run the script:
   ```
   python clear_temp_ram_etc.py
   ```
4. Use the GUI to click "Clean it" to start cleanup. Logs will display progress.
5. Click "Close" to exit the application.

### Running the Executable

1. Download or build the executable `clear_temp_ram_etc.exe` from the `dist` folder.
2. Run the executable. It will request administrator privileges.
3. Use the GUI as described above.

## Building the Executable

To build the executable yourself, use PyInstaller:

```
pyinstaller --onefile --windowed --icon=data-cleaning.ico --uac-admin clear_temp_ram_etc.py
```

This will create the executable in the `dist` folder.

## Notes

- Running the cleanup requires appropriate permissions; run as administrator if needed.
- The script is designed for Windows systems.
- The GUI uses CustomTkinter for a modern look.

## License

This project is open source and free to use.
