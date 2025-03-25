# Modern Countdown Timer

A sleek, modern countdown timer built with Python and Tkinter, designed for task tracking with Excel logging. Developed by Guth South Africa.

## Features

- **Customizable Timer**: Set countdowns up to 999 hours with intuitive hour, minute, and second spinboxes.
- **Job Tracking**: Log tasks with Job Number and Job Description fields.
- **Excel Logging**: Automatically saves pause and resume events to an Excel file in your Downloads folder, including pause duration.
- **Mini Window**: Displays a compact timer in the top-right corner when minimized.
- **State Persistence**: Saves timer state between sessions, allowing resumption on restart.
- **Modern UI**: Clean, dark-themed interface with Nord-inspired colors.

## Installation

### Prerequisites
- Windows operating system (tested on Windows 10/11).
- No additional software required for the pre-built installer.

### Using the Installer
1. **Download**: Grab the latest release from the [Releases](https://github.com/TravisMain/Artisan_Timer) page.
2. **Run**: Execute `setup.exe` and follow the setup wizard.
3. **Launch**: Open from the Start menu or desktop shortcut (if selected).

### From Source (Developers)
1. **Clone the Repository**:
   ```bash
   git clone (https://github.com/TravisMain/Artisan_Timer)
   cd ModernCountdownTimer

    Install Dependencies:
    bash

pip install openpyxl

    Python 3.9+ recommended.

Run:
bash
python ModernCountdownTimer.py
Build (Optional):

    Install PyInstaller: pip install pyinstaller.
    Compile with:
    bash

        pyinstaller --onefile --noconsole --add-data "path\to\openpyxl;openpyxl" --icon=timer.ico ModernCountdownTimer.py
        Replace path\to\openpyxl with your local openpyxl path (e.g., C:\Program Files\Python311\Lib\site-packages\openpyxl).

Usage

    Set Timer:
        Use the spinboxes to input hours, minutes, and seconds (up to 999:59:59).
    Enter Job Details:
        Fill in "Job Number" and "Job Description" (required to start).
    Start:
        Click "Start" to begin the countdown.
    Pause/Resume:
        Click "Pause" to halt; "Resume" to continue. Logs are saved to Downloads/[JobNumber]_[JobDescription].xlsx.
    Reset:
        Click "Reset" and confirm to clear the timer and start anew.
    Minimize:
        Minimize the window to see a mini timer in the top-right corner.

Excel Log Format

    File Location: C:\Users\YourName\Downloads\[JobNumber]_[JobDescription].xlsx
    Columns:
        Job Number
        Job Description
        State (Paused/Resumed)
        DateTime (e.g., 2025-03-24 12:34:56)
        Remaining Time (e.g., 000:05:23)
        Pause Duration (e.g., 00:01:45, empty for Paused)

Troubleshooting

    Excel File Not Saving:
        Check C:\Users\YourName\Downloads\timer_error.log for errors.
        Ensure no file with the same name is open in Excel.
        Verify openpyxl is bundled correctly if running from source or a custom build.
    Icon Missing:
        Ensure timer.ico is in the project folder or bundled with PyInstaller.

Building the Installer

    Install Inno Setup: Download from jrsoftware.org.
    Edit .iss File:
        Update paths in ModernCountdownTimer.iss to match your system.
    Compile:
        Open in Inno Setup Compiler and click "Build > Compile".
        Find ModernCountdownTimerSetup.exe in the installer folder.

License

This project is licensed under the MIT License - see the  file for details.
Contributing

Contributions are welcome! Please:

    Fork the repo.
    Create a feature branch (git checkout -b feature/YourFeature).
    Commit changes (git commit -m "Add YourFeature").
    Push to the branch (git push origin feature/YourFeature).
    Open a Pull Request.

Credits

    Developer: Guth South Africa
    Build: v1.0.0
    Tools: Python, Tkinter, openpyxl, PyInstaller, Inno Setup

Contact

For issues or suggestions, open an issue on GitHub or reach out via your - travis.m@guth.co.za.

Happy timing!
