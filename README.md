# Aurellium

Aurellium is a Windows desktop file organizer that helps you sort files by type with a guided, easy-to-use interface.

Pick a source folder, select file types with checkboxes, preview matching files, then move or copy them to your chosen destination.

## Download

- Latest release page: https://github.com/xoxogabweyl/Aurellium/releases/tag/v1.0.0
- Direct setup download: https://github.com/xoxogabweyl/Aurellium/releases/download/v1.0.0/Aurellium-Setup.exe

## Installation

1. Download `Aurellium-Setup.exe`.
2. Run the installer.
3. Launch **Aurellium** from Start Menu (or desktop shortcut if selected during install).

## Features

- Automatic file-type scanning from the selected source folder
- File-type checkboxes with per-type file counts
- Optional recursive scanning (`Include subfolders`)
- Destination modes:
- Move to an existing folder
- Create a new folder inside a parent folder
- Action modes:
- Move files
- Copy files
- Preview of matched files before processing
- Duplicate filename protection (`file.ext`, `file_1.ext`, `file_2.ext`, ...)
- Confirmation prompt before move/copy
- Operation log and warning summary
- Open destination folder after completion

## Quick Start

1. Choose a **Source folder**.
2. Click **Scan Types**.
3. Select scan option (**Include subfolders** on or off).
4. Choose **Mode**.
5. Set destination:
- Existing destination folder, or
- Parent folder + new folder name
6. Choose **Action** (`Move files` or `Copy files`).
7. Check the file types to process.
8. Optional: click **Preview Matches**.
9. Click the main action button.

## Safety Behavior

- Source and destination cannot be the same path.
- In recursive mode, files already inside the destination path are skipped.
- Existing destination files are not overwritten; a new unique name is created.
- If some files fail, Aurellium continues and reports failed items.

## Troubleshooting

- No file types found:
- Verify the source folder exists and contains files with extensions.
- Click **Scan Types** again.
- Files skipped:
- Check file permissions.
- Close apps that may be locking those files.
- Action cannot continue:
- Ensure at least one file type is checked.
- Ensure destination inputs are valid for the selected mode.

## Tech Stack

- Python
- PySide6
- PyInstaller
- Inno Setup
