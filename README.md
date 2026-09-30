# OmniWfn

OmniWfn opens the result file of a quantum-chemistry calculation and turns it into pictures and numbers. It shows where the electrons sit, how atoms bond, where a molecule will react and what light it absorbs. It does the work of the program [Multiwfn](http://sobereva.com/multiwfn/), with labelled buttons instead of menu numbers, draws publication-ready figures in place, and keeps every result.

**[Download the latest version](../../releases/latest)** · **[User Guide (PDF)](../../releases/latest/download/OmniWfn-User-Guide.pdf)**

This repository holds only the downloads. The source code is not public.

## Download and install (Windows 10 or 11, 64-bit)

Each release offers two downloads. Pick one:

| File | What it is |
| --- | --- |
| `OmniWfn-Setup-x.y.z.exe` | The installer. It adds OmniWfn to the Start menu and can be removed from Windows' app settings. |
| `OmniWfn-x.y.z.exe` | The portable version: a single program that runs without installing, for example from a USB stick. |

The downloads are not signed with a paid certificate, so Windows may show "Windows protected your PC" the first time. Click **More info**, then **Run anyway**.

## What you need

- **A finished calculation.** OmniWfn does not run quantum chemistry itself; it analyses the result. It opens:
  - Gaussian `.fchk` / `.fch`, or `.chk` if Gaussian's `formchk` is installed;
  - `.wfn` and `.wfx` files, and Multiwfn's `.mwfn`;
  - Molden files, for example from ORCA;
  - Gaussian and ORCA output files, cube files, and structure files (`.xyz`, `.pdb`, `.cif`), for the analyses that need only those.
- **Multiwfn (optional).** Almost every analysis runs in OmniWfn's own engine. A few menu functions, marked **Multiwfn**, need [Multiwfn](http://sobereva.com/multiwfn/), which you download separately and point to in Settings.

## What it does

- **Electron density and orbitals** in 3D: the orbitals, the density and its Laplacian, ELF and LOL, spin density and more.
- **Surfaces:** electrostatic potential and ionization energy mapped on the molecular surface, with their statistics and extreme points.
- **Weak interactions:** NCI, IRI and IGMH, with the scatter plot.
- **Atoms in molecules:** QTAIM critical points, bond paths and basins.
- **Charges:** Hirshfeld, CM5, ADCH, VDD, and RESP, MK and CHELPG fits.
- **Bond orders:** Mayer, Wiberg, Mulliken, fuzzy, Laplacian, IBSI and multicentre bonds.
- **Orbital composition and DOS** by atom, fragment and shell.
- **Localized orbitals** and oxidation states (LOBA).
- **Bonding between fragments:** CDA, ETS-NOCV and deformation densities. OmniWfn writes the fragment input files from your calculation.
- **Reactivity:** Fukui functions, the dual descriptor and conceptual-DFT indices.
- **Aromaticity:** HOMA, FLU, PDI, MCI, NICS, ICSS and ELF-π.
- **Spectra** from Gaussian and ORCA: IR, Raman, VCD, ROA, UV-Vis and ECD.
- **Excited states:** hole and electron, natural transition orbitals and charge transfer.
- **Sterics:** buried volume (%V_bur) and steric maps.
- **Structure:** distances, angles, and measurements to ring centres and planes.
- **Multiwfn by its keys:** every Multiwfn option is a button in the left panel. Keystroke Lookup finds an analysis from the keys you would type in Multiwfn, and warns when a key is not an option of the menu it is typed in. Multiwfn keystroke paths for QTAIM, fuzzy atoms and basins run in OmniWfn's own engine, with Multiwfn's menus and output.

Every figure can be edited and exported for print (TIFF, PNG, PDF or SVG, up to 1200 dpi). 3D scenes also export for 3D printing and as interactive web pages.

The numbers match Multiwfn's on the same files, and each native result shows the Multiwfn keystrokes that reproduce it. The [User Guide](../../releases/latest/download/OmniWfn-User-Guide.pdf) explains each analysis in plain words.

## License

OmniWfn is proprietary software. From version 0.3.0 on, it is licensed (not sold) under its **[End-User License Agreement](EULA.txt)**. The installer shows the agreement, and OmniWfn asks you to accept it the first time it starts. You may not copy, redistribute, modify or reverse-engineer OmniWfn. The components it is built on (Electron, Chromium, three.js) and the Multiwfn data and methods it uses keep their own licenses: see **[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt)**.

## Credit

OmniWfn reproduces methods implemented in Multiwfn by Tian Lu. If you publish results obtained with it, please also cite Multiwfn as its author asks, in the main text: T. Lu, F. Chen, *J. Comput. Chem.* 33, 580 (2012), and T. Lu, *J. Chem. Phys.* 161, 082503 (2024) ([sobereva.com/multiwfn](http://sobereva.com/multiwfn/)). OmniWfn is not affiliated with Multiwfn.
