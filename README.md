# YouSpot

YouSpot is a small downloader helper script that uses `youtube_dl`, `cfonts`, and `ffmpeg` to provide a simple menu for YouTube and Spotify downloads.

## Project Layout

- `newfile.py` - main menu-driven script.
- `Termux/Python.sh` - installs dependencies and prepares the Termux flow.
- `Cd/termux.sh` - copies the script into Termux downloads and runs it.
- `Linux/python.sh` - installs dependencies for Debian/Ubuntu-based systems.

## Requirements

- Python 3
- `pip`
- `youtube_dl`
- `python-cfonts`
- `ffmpeg`
- Termux storage access if you are using Android

## Termux

1. Open the project folder in Termux.
2. Run the setup script:

```bash
cd YouSpot/Termux
bash Python.sh
```

3. After the setup finishes, run:

```bash
bash termux.sh
```

The Termux flow copies `newfile.py` into your downloads folder and starts the downloader menu from there.

## Linux / Debian / Ubuntu

1. Open a terminal in the project folder.
2. Install the dependencies with:

```bash
cd Linux
bash python.sh
```

3. Run the main script from the project directory:

```bash
python newfile.py
```

## Notes

- The scripts are written around the current folder structure in this repository.
- If you change the location of `newfile.py`, update the helper scripts as well.
- Some commands in the helper scripts assume elevated permissions or a working network connection.
