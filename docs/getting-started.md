# Getting started

## Requirements

- Autodesk Revit 2022 or 2024, matching the installer you downloaded
- Windows 10 or 11, 64-bit
- A per-user install. Administrator rights are not required

## Install

1. Close Revit.
2. Run `LOD++-Setup-Revit<year>-<version>.exe`.
3. Start Revit. The **LOD++** tab loads for the Windows user who ran the setup.

An unsigned build may show **Unknown publisher** in Windows SmartScreen. For a build you trust, choose **More info**, then **Run anyway**.

## First session

| Task | Command |
|------|---------|
| Version and license | **LOD++ → About** |
| Room, level, or coordinate values | **Information++ → Locate** |
| Parameter values from a rule or a spreadsheet | **Information++ → Populate** |
| Unused families and types | **Audit++ → Purge++** |
| Text notes | **System++ → Find & Replace** |

Read [Using LOD++](using-lodpp.md) before the first write. **?** on a command opens its page.

## Uninstall

Windows **Settings → Apps → LOD++ (Revit 20xx) → Uninstall**.

This removes the add-in manifest and the files under `%LOCALAPPDATA%\LOD++`.
