#  Exploring Universe With JWST

An interactive website documenting research carried out during **TIFR's NIUS 2025** (National Initiative on Undergraduate Science) programme — covering astronomical image processing and exoplanet transit detection, built from scratch with HTML/CSS/JS and interactive canvas visualizations.

> Selected as 1 of ~35 students nationally for TIFR's undergraduate science research programme. This site walks through the methods, code, and findings from that work.

##  What's inside

### [`index.html`](index.html) — Home
Landing page introducing the project and linking out to each module.

### [`imageprocessing.html`](imageprocessing.html) — Astronomical Image Processing
CCD image calibration pipeline, built interactive:
- **Master Bias Frame Creation** — removing read-out noise from raw CCD frames
- **Aperture Photometry** — with an adjustable-parameter interactive demo
- **Image Subtraction (ILMT Data)** — interactive reference-vs-difference image comparison for transient detection
- **Complete CCD Calibration Pipeline** — bias and flat-field correction end-to-end

### [`Simulation_Transient_Curve.html`](Simulation_Transient_Curve.html) — Transit Light Curve Analysis
A full walkthrough of detecting an exoplanet from light-curve data:
- Loading and cleaning real **TESS data (WASP-100)**
- **PLD systematics correction**
- **Box Least Squares (BLS)** algorithm for period finding
- Transit modelling with **`batman`**, parameter fitting via `curve_fit`
- **MCMC posterior sampling** for parameter uncertainty

### [`Blogs.html`](Blogs.html) — Field Blogs & Research Notes
Write-ups from the research process, including:
- Detecting an Exoplanet Transit with TESS & Batman
- Why Your Telescope Images Look Terrible (& How to Fix Them)
- Reading the Sun: Coronal Loops & Active Regions with SunPy
- Understanding the BLS Periodogram — Hunting Planets in Noise
- Image Subtraction on ILMT Data — Finding the Invisible
- What the Transit Depth Tells You — Inferring Planetary Properties
- JWST: Two Years of Science and What Comes Next

## Built with

Vanilla HTML, CSS, and JavaScript — including hand-built canvas visualizations for the interactive photometry and image-subtraction demos (no external charting libraries).

Underlying analysis was done in Python using `lightkurve`, `batman`, `ccdproc`, `photutils`, `astroalign`, and `sunpy`.

##  Background

This project grew out of research on exoplanet detection via the Transit Method during TIFR's NIUS programme — modelling stellar light curves, processing CCD imaging data (bias/flat-field correction), and detecting transient objects through image subtraction and alignment.

##  Author

**Mann Sutariya** — B.Sc Physics, PDEU
 mannsutaria2605@gmail.com
