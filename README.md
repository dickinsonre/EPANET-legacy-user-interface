CONTENTS
========

This repository contains source code for EPANET2W Delphi 
Windows application. The code is contained in the
following folders:

  components.zip -- Custom Delphi components that must be
                    installed into the Delphi IDE's component
                    palette before working with the GUI code.
                    Files last updated on 7/5/06.

  epanet2w.zip  -- Borland Delphi code that comprises the
                   graphical user interface (GUI) for the
                   Windows version of EPANET 2. Should be
                   compiled into an executable named epanet2w.exe
                   for use with the EPANET program. Files last
                   updated on 2/25/08.


# EPANET Legacy User Interface

A preserved Delphi-based graphical user interface for the Windows version of EPANET, maintained as a fork of the U.S. EPA legacy repository for reference, archival, and possible recompilation work. The repository contains the source code for **EPANET2W**, the classic Windows GUI used with EPANET's water distribution system simulation engine.[1][2][3]

## Overview

This repository archives the legacy Pascal/Delphi code for the EPANET Windows desktop interface rather than the newer cross-platform EPANET GUI. The codebase is a fork of `USEPA/EPANET-legacy-user-interface`, and the current GitHub page shows it as up to date with the upstream `master` branch.[1][2]

The main purpose of the repository is to preserve the historical GUI implementation and support users who want to inspect, rebuild, or study the original Windows interface. EPA describes EPANET itself as a software application for modeling drinking water distribution systems, including hydraulic and water quality behavior over time.[4][5]

## What this repository contains

The repository currently consists of two principal source folders plus a minimal root README.[1]

| Folder | Purpose |
|---|---|
| `components/` | Custom Delphi components that must be installed into the Delphi IDE before working with the GUI code.[1][6] |
| `epanet2w/` | Borland Delphi source code for the EPANET2W Windows graphical user interface, intended to compile into `epanet2w.exe`.[1][2][3] |

According to the repository README shown on GitHub, the component files were last updated on 2006-07-05 and the EPANET2W GUI files were last updated on 2008-02-25.[1] The language breakdown on GitHub shows the codebase as 100% Pascal, which is consistent with the Delphi implementation.[1]

## Relationship to EPANET

EPANET is used to simulate pressurized water distribution systems, including pipes, junctions, pumps, valves, tanks, and reservoirs, while tracking hydraulic conditions and water quality over extended periods.[4][5] The legacy GUI in this repository provided the classic Windows environment for building network models, editing data, running analyses, and reviewing results.[4][3]

This repository is best understood as the historical user-interface layer, not the current canonical EPANET engine repository. EPA and the broader EPANET ecosystem now also reference newer codebases and documentation, including EPANET 2.2 documentation and newer GUI efforts.[7][8][9]

## Build notes

To work with the GUI source, the Delphi custom components need to be compiled and installed before loading the main EPANET2W project into the IDE.[1][10][3] External guidance for compiling the EPANET GUI with modern Delphi Community Edition describes this sequence:

1. Download or clone the GUI source and required toolkit files.[10]
2. Build and install the custom components from the `components` folder in Delphi.[10][3]
3. Open the EPANET2W project in the `epanet2w` folder.[10][3]
4. Configure Delphi library paths so the GUI project can resolve both the component sources and generated build outputs.[10]
5. Compile the application to produce the Windows executable.[10][3]

Because this repository is a legacy code archive, modern build steps may require adaptation depending on the Delphi version, local library paths, and the EPANET engine DLL arrangement.[10][11]

## Suggested prerequisites

Anyone attempting to build or modify this code should expect to need:

- A Delphi-compatible Windows development environment, because the code is written in Pascal/Delphi.[1][10][11]
- Installed custom components from the `components` folder before opening the GUI project.[1][6][3]
- Familiarity with EPANET's Windows GUI concepts and network modeling workflow.[4][5]
- Access to the EPANET engine files used by the GUI during execution or testing.[10][3]

## Repository status

The visible repository metadata indicates a small historical code archive with three commits, one branch, no tags, no releases, and no packages published at the time the page was viewed.[1] GitHub also identifies this repository as a public fork of `USEPA/EPANET-legacy-user-interface`.[1][2]

That status suggests the repository is primarily archival rather than an actively evolving application. It is useful for historical reference, source inspection, and specialized maintenance work on the classic EPANET interface.[1][2]

## Recommended README additions for GitHub

If the goal is to make the repository more useful to other EPANET developers and historians, the README would benefit from several practical additions:

- A short explanation of how this legacy GUI differs from newer EPANET repositories and user interfaces.[8][5][9]
- Explicit build instructions for a known Delphi version, including required packages, search paths, and expected output executable.[10][3]
- Notes on whether the repository is intended only for archival use or also for active experimentation.[1][2]
- A dependency note describing how the GUI interacts with the EPANET engine DLL and any expected external files.[10][3]
- Screenshots of the classic interface, if available, to help users understand what is being preserved.[4][3]

## Expanded README draft

Below is a stronger GitHub-facing README draft you could use directly in the repository:

***

# EPANET Legacy User Interface

This repository preserves the Delphi/Pascal source code for **EPANET2W**, the classic Windows graphical user interface used with EPANET. It is a fork of the U.S. EPA legacy repository and is intended for archival reference, source inspection, and possible rebuilding of the historical desktop application.[1][2][3]

## Purpose

The project captures the original Windows GUI layer for EPANET, the widely used water distribution system modeling software developed by the U.S. EPA. While newer EPANET repositories and interfaces now exist, this codebase remains valuable for understanding the historical implementation of the classic EPANET desktop experience.[4][8][5]

## Repository contents

- `components/` — custom Delphi components required by the GUI project; these must be installed into the Delphi IDE before opening or compiling the EPANET2W application.[1][6][3]
- `epanet2w/` — source code for the Windows GUI application, typically compiled into `epanet2w.exe`.[1][2][3]

## About EPANET

EPANET is a simulation program for pressurized drinking water distribution systems. It can analyze hydraulic performance and water quality behavior in networks consisting of pipes, nodes, pumps, valves, tanks, and reservoirs over an extended simulation period.[4][5]

## Build overview

To rebuild the legacy GUI, the Delphi component library should be installed first, then the EPANET2W project can be opened and compiled. Modern Delphi environments may require manual path configuration for the component packages and any required EPANET engine files.[10][3]

Typical workflow:

1. Open the Delphi project in `components/` and compile, build, and install the custom components.[10][3]
2. Open the EPANET2W project in `epanet2w/`.[10][3]
3. Configure the Delphi library paths to include the component directories and any generated release folders.[10]
4. Ensure required EPANET toolkit files are available to the GUI project.[10][3]
5. Compile the application and verify that the Windows executable runs correctly.[10]

## Notes

- This is a **legacy** codebase and may require adjustments to compile in current Delphi environments.[10][11]
- The repository is best viewed as an archival source tree unless additional maintenance work is planned.[1][2]
- For current EPANET development, consult newer EPA or community-maintained repositories and documentation.[7][8][5][9]

## Upstream source

Original upstream repository: [USEPA/EPANET-legacy-user-interface](https://github.com/USEPA/EPANET-legacy-user-interface) [2]

Related EPANET resources:

- [EPA EPANET overview](https://www.epa.gov/water-research/epanet) [4]
- [EPANET 2.2 documentation](https://usepa.github.io/EPANET2.2/) [7]
- [Current EPANET GUI repository](https://github.com/USEPA/EPANET) [8]

***



