# Aurellium

Aurellium is a Windows desktop file organizer that lets you sort files by type using a simple guided UI.

You choose a source folder, scan available file types, select what you want, preview matches, then move or copy files to a destination.

## App Highlights

- Automatic file-type detection from the selected source folder
- Checkbox-based type selection with per-type file counts
- Optional recursive scan using `Include subfolders`
- Destination modes: `Move to this folder` or `Create a new folder`
- Actions: `Move files` or `Copy files`
- Preview before processing
- Duplicate filename protection (`name.ext`, `name_1.ext`, `name_2.ext`, ...)
- Confirmation prompts, operation logs, and warning reporting
- One-click `Open Destination` after processing

## Download and Install

Direct download:

- [Download Aurellium Setup](https://github.com/xoxogabweyl/Aurellium/raw/main/Aurellium-Setup.exe)

Install steps:

1. Download `Aurellium-Setup.exe` using the link above.
2. Run the installer.
3. Open **Aurellium** from Start Menu (or Desktop if that option was selected).
## Quick Start

1. Set **Source folder**.
2. Click **Scan Types**.
3. Enable or disable **Include subfolders**.
4. Choose **Mode**.
5. Set **Destination folder** (or parent + new folder name in create mode).
6. Choose **Action** (`Move files` or `Copy files`).
7. Check the file types you want.
8. Optional: click **Preview Matches**.
9. Click the main action button to run.

## Mode Guide

- `Move to this folder`: selected files go directly into the destination folder.
- `Create a new folder`: app creates a folder inside the parent folder, then places selected files there.

## Safety Rules

- Source and destination cannot be the same path.
- In recursive scans, files already under the destination path are skipped.
- Existing files in destination are never overwritten; new names are generated automatically.
- You get a confirmation dialog before move/copy starts.
- If some files fail, Aurellium continues and reports the failures in the log.

## Troubleshooting

- No file types detected: verify source folder and click **Scan Types** again.
- Files skipped: check file permissions or whether another app is locking those files.
- Action blocked: ensure destination is valid and at least one type is selected.

## Built With

- Python
- PySide6
- PyInstaller
- Inno Setup

