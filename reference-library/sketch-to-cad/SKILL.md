---
name: sketch-to-cad
description: Convert hand-drawn sketches, scanned drawings, or photographed sketches into structured, editable 2D CAD geometry. Use this skill when the user wants to turn a hand sketch into CAD, DXF, DWG, a dimensioned drawing, or a clean CAD reference. Prefer dimensionally constrained reconstruction over literal tracing.
---

# Sketch to CAD

Turn a hand-drawn sketch into clean, editable CAD geometry while preserving the intended design.

## Goal

Create a CAD-ready reconstruction that is:
- dimensionally consistent
- editable
- organized by logical layers
- faithful to the design intent
- validated before export

## Before starting

Inspect the source and determine:
- drawing type: architectural, interior, furniture, product, mechanical, or general diagram
- visible geometry: lines, polylines, circles, arcs, openings, symbols
- dimensions and units
- text and annotations
- construction/reference lines
- ambiguous or missing information
- whether the source is a scan or a photograph

If the drawing is photographed, account for rotation, perspective distortion, shadows, and uneven scaling before using it as a geometric reference.

## Scale and dimensions

A reliable real-world dimension is required for a dimensionally accurate result.

Use known dimensions to establish scale. If several known dimensions conflict, flag the conflict instead of silently choosing one.

Never invent missing dimensions.

If no reliable dimension is available:
- produce only a proportional/reference reconstruction
- clearly mark the result as unscaled
- do not present estimated dimensions as factual

## Reconstruction rules

Do not blindly trace every hand-drawn stroke.

Reconstruct the intended CAD geometry:
- make intended horizontal elements horizontal
- make intended vertical elements vertical
- preserve parallel and perpendicular relationships
- use exact circles and arcs where intended
- join related segments into clean polylines
- remove duplicate, accidental, or insignificant strokes
- preserve symmetry and repetition when clearly intended
- prioritize explicit dimensions over visual estimation

Treat dimension lines, arrows, handwritten notes, and construction marks as annotations unless the sketch clearly indicates that they are geometry.

## Recommended layers

For architectural/interior drawings:
- A-WALL
- A-DOOR
- A-WINDOW
- A-FURN
- A-DIM
- A-TEXT
- A-HATCH
- A-CONSTRUCTION

For mechanical/product drawings:
- M-PROFILE
- M-HOLE
- M-CENTER
- M-DIM
- M-TEXT
- M-CONSTRUCTION

Use the simplest layer structure appropriate to the drawing. Do not create unnecessary layers.

## Validation

Before export, verify:
- known reference dimensions
- overall width and height
- wall or profile thickness where applicable
- horizontal and vertical alignment
- parallelism and perpendicularity
- intersections and joins
- closed profiles where required
- duplicate or disconnected geometry
- layer assignment
- units and scale
- unresolved ambiguities

Separate confirmed geometry from estimated or ambiguous geometry.

## Output

Prefer:
1. editable CAD geometry
2. DXF as the primary exchange format
3. DWG when a DWG-capable workflow is available
4. a concise validation summary

The validation summary should state:
- drawing type
- units
- scale/reference dimension
- what was reconstructed
- unresolved ambiguities
- validation status

## Quality principle

The objective is not to make the CAD file look like the hand drawing.

The objective is to recover the intended geometry and dimensions represented by the hand drawing, while making uncertainty explicit.
