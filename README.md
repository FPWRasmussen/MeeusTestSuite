# MeeusJS Comprehensive Test Suite

This repository contains an HTML-based test suite designed to comprehensively evaluate the `MeeusJS` astronomical calculation library (v1.0.4 from Skypack CDN). It runs a series of calculations for various astronomical phenomena, times, and locations, displaying the results directly in the browser.

## Features

*   **Live Testing:** Executes MeeusJS functions directly in your browser.
*   **Comprehensive Checks:**
    *   Time conversions (Julian Day, MJD, DeltaT).
    *   Earth orientation parameters (Nutation, Obliquity, Sidereal Time).
    *   Solar position (topocentric Az/Alt, RA/Dec) for multiple global locations.
    *   Equation of Time.
    *   Solar rise, transit, and set times, including day length and local mean time conversions.
    *   Polar day/night determination.
    *   Atmospheric refraction model comparison (Bennett & Saemundsson).
    *   Coordinate utility tests.
    *   Lunar position (topocentric Az/Alt, RA/Dec), distance, parallax, angular diameter.
    *   Moon phase (angle, illuminated fraction, name).
    *   Lunar rise, transit, and set times.
    *   Mean solar parallax and semidiameter.
    *   Basic tests of the `Rise` module functions (circumpolar, approxTransit).
*   **Clarity on Constants:** Uses constants directly from the MeeusJS library where available (e.g., `A.AU`, `A.Globe.Er`) and clearly indicates when standard script-defined values are used for those not directly exported (e.g., Solar/Lunar physical radii).
*   **Detailed Output:** Results are formatted for readability in an HTML `pre` tag, with color-coding for different data types.
*   **Performance Metrics:** Includes a basic performance test for solar position calculations.
*   **Statistics:** Summarizes the number of tests run, successes, and failures.
*   **Exportable Results:** Allows users to download the raw test output as a text file.

## Purpose

This suite aims to:
1.  Verify the accuracy and consistency of MeeusJS calculations against expected astronomical behavior and standard formulas (like those found in Jean Meeus' "Astronomical Algorithms").
2.  Demonstrate the usage of various modules within the MeeusJS library.
3.  Provide a clear, live view of the library's capabilities.
4.  Serve as a debugging and validation tool for the MeeusJS library.

## How to Use

1.  Clone this repository or download the HTML file (e.g., `index.html`).
2.  Open the HTML file in a modern web browser that supports ES modules (e.g., Chrome, Firefox, Edge, Safari).
3.  Click the "🔄 Run/Refresh Tests" button to execute the test suite.
4.  Results will be displayed on the page.
5.  You can use the "📥 Export Results" button to save the output.

## MeeusJS Library

This test suite specifically targets `meeusjs@1.0.4` as imported from `https://cdn.skypack.dev/meeusjs@1.0.4`. MeeusJS itself is a JavaScript implementation of astronomical algorithms, largely based on the work of Jean Meeus.

## Disclaimer

While this test suite is comprehensive, it is primarily designed for validation and demonstration. For critical applications, always cross-verify results with other established astronomical sources or software. The "manual" calculations (like Equation of Time) are based on standard formulas but are implemented within this test script for comparison or when not directly provided by a single library function.

## Contributions

Feel free to fork, modify, or suggest improvements to this test suite.