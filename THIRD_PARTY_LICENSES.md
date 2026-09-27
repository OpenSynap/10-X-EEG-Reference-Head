# Third-Party Licenses and Notices

This file documents third-party material that materially contributed to the public **10-X EEG Reference Head** release, together with sources used for EEG nomenclature and methodology.

It is a provenance and attribution record, not legal advice. Third-party material remains subject to its original terms. The project license applies only to OpenSynap's own contributions and does not replace third-party terms.

## 1. ICBM152 Extended 2020 asymmetric

**Role in this project:** Primary anatomical source for the reference head/scalp geometry.

**Source:** Montreal Neurological Institute (MNI), McConnell Brain Imaging Centre, McGill University  
**Dataset:** ICBM152 Extended 2020 asymmetric  
**Official source:** https://www.bic.mni.mcgill.ca/~vfonov/icbm/2020/

The released reference-head surface was derived from the asymmetric ICBM152 Extended 2020 anatomical volume. The original archive includes a `COPYING` notice. This repository preserves that notice and does not make any broader legal claim about the source files beyond the terms supplied with the original archive.

The bundled notice reads:

> Copyright (C) 1993-2020 Louis Collins, McConnell Brain  
> Imaging Centre, Montreal Neurological Institute, McGill University.  
> Permission to use, copy, modify, and distribute this software and  
> its documentation for any purpose and without fee is hereby granted,  
> provided that the above copyright notice appear in all copies.  
> The authors and McGill University make no representations about the  
> suitability of this software for any purpose. It is provided "as is"  
> without express or implied warranty. The authors are not responsible  
> for any data loss, equipment damage, property loss, or injury to  
> subjects or patients resulting from the use or misuse of this  
> software package.

Because the notice uses the wording “software and its documentation,” this file intentionally avoids extending or reinterpreting that wording. Users who require a formal determination of rights in the original atlas data should review the terms distributed with the source archive or contact the rights holder.

## 2. `eeg_positions`

**Role in this project:** Coordinate-free EEG position-name inventories and cross-checking of 10-X nomenclature. Source XYZ coordinates were not used as canonical coordinates for this project.

**Project:** `eeg_positions`  
**Repository:** https://github.com/sappelhoff/eeg_positions  
**Zenodo:** https://doi.org/10.5281/zenodo.3718568  
**License:** MIT License

Required notice from the upstream project:

> Copyright (c) 2018 eeg_positions developers

The upstream MIT license applies to material taken from that project. The final OpenSynap coordinates were independently generated on the reference scalp and were not copied from the upstream XYZ values.

## 3. EEG standards and literature

The following publications were used as nomenclature, measurement, or methodological references. No article figures, page images, or substantial article text are redistributed in this repository.

- **Jasper HH (1958)** — original International 10-20 proposal.  
  DOI: https://doi.org/10.1016/0013-4694(58)90053-1

- **Klem GH, Lüders HO, Jasper HH, Elger C (1999)** — IFCN description of the 10-20 system.  
  PubMed: https://pubmed.ncbi.nlm.nih.gov/10590970/

- **Acharya JN, Hani A, Cheek J, Thirumala P, Tsuchida TN (2016)** — ACNS Guideline 2: Guidelines for Standard Electrode Position Nomenclature.  
  DOI: https://doi.org/10.1097/WNP.0000000000000316  
  ACNS guidelines page: https://www.acns.org/practice/guidelines

- **Oostenveld R, Praamstra P (2001)** — the 10-5 extension.  
  DOI: https://doi.org/10.1016/S1388-2457(00)00527-7

These works are cited as references only. This repository does **not** redistribute the ACNS figure used during research, nor a figure-derived transcription file. The public coordinate files contain the project's own generated coordinates paired with standard electrode names.

## 4. Development and QA sources not included in the public release

Several third-party datasets were inspected during development or used for comparison/QA. Their source meshes, scans, article PDFs, and other original files are **not distributed in this public repository**, and no source triangles from the items listed below are included in the released reference-head mesh.

### RWTH adult head-and-torso scan

Hark Simon Braren and Janina Fels (2020), *A High-Resolution Individual 3D Adult Head and Torso Model for HRTF Simulation and Validation: 3D Data*.  
DOI: https://doi.org/10.18154/RWTH-2020-06760

Used during development as lower-head/neck shape guidance and comparison. No RWTH donor triangles are distributed in the final mesh.

### HUTUBS

Brinkmann et al., *The HUTUBS head-related transfer function (HRTF) database*.  
DOI: https://doi.org/10.14279/depositonce-8487

Used in rejected ear-shape experiments and visual/anatomical comparison. No HUTUBS donor triangles or HUTUBS files are distributed in the final release.

### HSRD-100

Digital Reality Lab, *HSRD-100: 100 High-Quality 3D Human Scans Dataset from HumanScanRepository*.  
Source: https://huggingface.co/datasets/digitalrealitylab/HSRD-100

Inspected as a possible anatomical donor/reference during research. No HSRD-100 geometry or files are included in the released model.

### openSAHE

Moura FS, Beraldo RG, Ferreira LA, Siltanen S, *openSAHE: Open Source Statistical Anatomical Atlas of the Human head for Electrophysiology Applications (precomputed atlases)*.  
DOI: https://doi.org/10.5281/zenodo.5559624

Used for earlier comparison/QA. No openSAHE mask or derived surface is distributed in the final release.

## 5. What this repository redistributes

The public repository is intended to contain only:

- the released 10-20, 10-10, and 10-5 reference-head models;
- the bare reference-head model;
- project-generated coordinate CSV files;
- project-generated renders;
- the project README, license, and attribution/notices files.

Research archives, third-party source datasets, downloaded papers, source-page snapshots, and internal development material are intentionally excluded.

## 6. Project license

OpenSynap's original contributions are released under the license stated in the repository's `LICENSE` file.

That project license does not cancel, replace, or broaden any rights or obligations associated with third-party source material. Where a released asset is derived from third-party material, the applicable upstream notice and attribution should be retained together with the project license.

