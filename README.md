# SolarTrack3D

A Python-based 3D solar shadow projection and dynamic tracking engine built with `pvlib` and `shapely` for PV panel shading analysis, area consumption calculations, and tilt/azimuth optimization.
3D solar shadow projection and dynamic tracking engine built with pvlib and shapely for PV panel shading analysis and tilt/azimuth optimization.

## Key Features

- **Solar Position Engine:** Uses `pvlib` for precise zenith, elevation, and azimuth computations based on location coordinates and timestamps.
- **3D-to-2D Shadow Projection:** Maps 3D obstacle vertices onto arbitrary panel surface planes using `shapely` vector math and polygon intersections.
- **Surface Area Consumption:** Calculates real-time shaded vs. unshaded panel surface area ($m^2$) and total coverage percentage.
- **Dynamic Tracking Adjustments:** Computes hourly tilt and azimuth delta movements required to maintain optimal direct solar exposure.
- **Environmental Irradiance:** Supports low-irradiance and cloudy condition modeling via ambient light factors (`ghi_factor`).

## Project Structure

```text
Enercog/
├── solarmodel.ipynb      # Base 3D shadow projection and irradiance engine
├── SolarModel2.ipynb     # Dynamic tracking, area consumption, and time-series loop
└── README.md             # Project documentation
