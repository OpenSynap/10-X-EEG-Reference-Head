# 10-X EEG Reference Head

An open 3D reference head for EEG electrode positioning across the **10-20, 10-10, and 10-5 systems**.

The project is intended for EEG researchers, developers, students, and enthusiasts who need reusable 10-X electrode reference geometry on an anatomically averaged human head model.

Published by **OpenSynap**, but designed as a general-purpose resource and not tied to OpenSynap hardware.

## Available reference sets

| System | Recording sites |
|---|---:|
| 10-20 | 19 |
| 10-10 | 71 |
| 10-5 | 339 |

The 10-5 model uses the explicitly defined **339-site scalp subset** accepted for this project. It does not treat every label found in generic 10-5 inventories as a physical scalp recording site.

## 3D model downloads

The full 3D model files are distributed through the repository's **GitHub Releases**.

Available model packages include:

- 10-20 reference head
- 10-10 reference head
- 10-5 reference head
- bare reference head

Where available, releases also include labeled and sites-only variants in formats such as **BLEND, STL, OBJ, and PLY**.

Use the **Releases** section of this repository to download only the model files you need.

## Coordinates and renders

Canonical electrode coordinates and reference renders are available directly in the repository.

The coordinate files provide the released 10-20, 10-10, and 10-5 site positions, while the render images provide visual references from multiple viewing angles.

The CSV coordinates are the canonical reference data. Marker meshes, labels, and rendered images are visualization assets and should not be used to regenerate canonical coordinates.

## Sources and methodology

The base head geometry was derived primarily from the **ICBM152 Extended 2020 asymmetric** anatomical dataset.

ICBM152 was selected because it provides an adult population-average anatomical reference in standardized MNI space, making it suitable as a reproducible scalp-reference geometry.

EEG positions were generated on the head surface from fiducials, measured scalp contours, and surface arc-length fractions. Published template XYZ coordinates were not used as the canonical placement method.

The placement and nomenclature work was based on established sources for the 10-X family, including:

- Jasper (1958) — International 10-20 system
- Klem et al. (1999) — IFCN 10-20 description
- ACNS Guideline 2 — 10-10 nomenclature
- Oostenveld & Praamstra (2001) — 10-5 extension

Third-party datasets, literature, licenses, and their roles in the project are documented in [`THIRD_PARTY_LICENSES.md`](THIRD_PARTY_LICENSES.md).

## Coordinate system

Canonical coordinates use:

- **MNI RAS+**
- **millimetres**

## Known limitations

This project is an **EEG scalp-reference model**, not a claim of full anatomical validation of an entire human head.

Known upstream limitations include:

- the natural chin / upper-neck region remains under a formal anatomical HOLD;
- the inion is an atlas-surface estimate with documented contour caveats;
- the dense 10-5 model is a coordinate/reference visualization, not a physical EEG-cap fit validation.

These limitations do not change the released, locked scalp-coordinate sets.

## AI-assisted development

Development was AI-assisted.

- **GPT-6 Sol** was used primarily for geometry/modeling workflows, implementation, validation, and QC.
- **Luna** was used primarily for literature review, source discovery, and research support.

Final outputs and acceptance decisions were manually reviewed before release.

## License

Unless otherwise noted, OpenSynap's original contributions in this repository are released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

See [`LICENSE`](LICENSE) for the license text.

Third-party source material remains subject to its original license and attribution requirements. See [`THIRD_PARTY_LICENSES.md`](THIRD_PARTY_LICENSES.md) for details.
