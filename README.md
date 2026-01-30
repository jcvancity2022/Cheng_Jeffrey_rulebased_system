#Cheng_Jeffrey_rulebased_system
Overview

Cheng_Jeffrey_rulebased_system is a rule‑based generative architecture and visualization system built in Python using Matplotlib. The project explores liminal architecture by algorithmically constructing a resort‑above / mall‑below megastructure inspired by real‑world courtyard resorts (e.g. RIU‑style hotels).

The system emphasizes:

Clear architectural hierarchy (center mass → folded wings)

Courtyard‑based perspective (not classical single‑point perspective)

Cubic, modular logic over freeform shapes

Readability and structural coherence over photorealism

This is not a renderer or game engine. It is a diagrammatic architectural system meant for conceptual design, research, and computational creativity.

Key Concepts
1. Rule‑Based Architecture

The system relies on explicit rules instead of randomness:

Fixed bay widths and floor heights

Center‑first massing logic

Wings fold inward using hinge‑style transforms

Mall and resort share a single structural axis

2. Courtyard Perspective

Rather than a traditional vanishing‑point camera, the project uses a courtyard convergence model:

All side wings subtly converge toward the courtyard center

Perspective strength increases with vertical depth

Prevents pyramid distortion while preserving depth

This produces a believable resort courtyard view similar to real hotel photography.

3. Center + Wing Hierarchy

Both the resort and mall follow the same spatial logic:

Center block: flat, orthographic, dominant

Wings: folded inward, scaled by depth

Podium: structural hinge between hotel and mall

This shared logic is what visually integrates the two programs into a single megastructure.

System Structure
Core Components

perspective_x()

Handles all perspective transformations

Supports courtyard convergence

Ensures consistent depth scaling across systems

draw_resort_facade()

Generates the main hotel mass

Flat central block + inward‑folding wings

Window rhythm based on architectural bays

draw_cubic_wing_detail()

Adds stepped, cubic articulation to wings

Floor‑by‑floor setbacks for depth and realism

Mall integration block

Central mall mass aligned with hotel center

Folded mall wings matching hotel logic

Structural continuity with podium

Visual Language

Color coding

Sand / tan: resort and podium

Steel blue: mall structure

Muted greens: landscape accents

Line weights

Thicker lines = primary structure

Thinner lines = secondary articulation

Abstraction level

Intentional diagrammatic style

Avoids textures, materials, and lighting

Focuses on massing and proportion

Requirements

Python 3.9+

matplotlib

numpy (optional but recommended)

This project runs entirely locally and does not require GPU acceleration.

Usage

Open the main notebook or Python script

Run all cells from top to bottom

The system outputs a high‑resolution architectural diagram:

liminal_resort_mall.png

You may safely adjust:

Number of floors

Bay widths

Courtyard convergence strength

Mall depth and width

Avoid changing perspective math unless you understand the hierarchy.

Design Intent

This project sits at the intersection of:

Computational creativity

Architectural diagramming

Generative systems

Liminal spatial design

It is designed to be readable, explainable, and rule‑driven, rather than stochastic or AI‑generated.

Author

Jeffrey Cheng
Interactive Arts & Technology (SIAT)
Simon Fraser University

License

This project is provided for educational and research purposes. Attribution is appreciated if reused or extended.
