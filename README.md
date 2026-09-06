# SolarModel
A Python-based 3D-to-2D solar shadow projection engine using pvlib and shapely to calculate shading coverage and effective solar exposure on tilted PV panels.

# SolarModel: Solar Panel Shadow Projection Engine

SolarModel is a Python-based geometric modeling tool designed to calculate shading percentages and effective irradiance on tilted solar panels caused by 3D obstacles.

## Features
- **Solar Position Calculation:** Integrates `pvlib` for precise zenith and azimuth tracking based on coordinates and timestamps.
- **Geometric Shadow Projection:** Maps 3D obstacle vertices onto a 2D panel plane using `shapely` convex hulls and polygon intersections.
- **Irradiance & Partial Shading Support:** Accounts for diffuse light and low-irradiance conditions via `ghi_factor`.
- **Edge Case Error Handling:** Handles parallel light rays, off-panel shadow projections, and degenerate geometries safely.

## Dependencies
- `numpy`
- `pandas` (>= 2.2.0)
- `pvlib`
- `shapely`

## Installation & Setup
```bash
pip install numpy pandas pvlib shapely
