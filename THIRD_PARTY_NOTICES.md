# Third-Party Notices

This file records source provenance and the terms documented in this repository. It is not legal advice. The versioned model release is under [`release/neuropen_reference_head_v1/`](release/neuropen_reference_head_v1/); the wider checkout also contains research and QA material under `materials/`. A source being listed here does not mean its geometry is part of the final model.

## Sources contributing to final outputs

### ICBM152 Extended 2020 asymmetric — primary head geometry

- **Source / owner:** `icbm152_ext55_model_asym_2020_nifti.zip`, dataset `icbm152_ext55_model_asym_2020`; Montreal Neurological Institute, McConnell Brain Imaging Centre, McGill University.
- **Official source:** [MNI 2020 archive index](https://www.bic.mni.mcgill.ca/~vfonov/icbm/2020/) · [Exact NIfTI archive](https://www.bic.mni.mcgill.ca/~vfonov/icbm/2020/icbm152_ext55_model_asym_2020_nifti.zip).
- **Use:** The final head’s cranial/scalp and facial reference geometry is derived from the archive’s asymmetric T1 volume. The local left-ear correction uses the contralateral ICBM source form.
- **License / terms:** The exact archive contains `COPYING`. It grants permission to use, copy, modify, and distribute the software and its documentation for any purpose and without fee, provided the copyright notice appears in all copies. The notice also contains an “as is” warranty disclaimer and liability disclaimer. The project retains that notice in the final release. No SPDX license identifier is stated in the bundled text.
- **Required notice:** “Copyright (C) 1993-2020 Louis Collins, McConnell Brain Imaging Centre, Montreal Neurological Institute, McGill University.”
- **Local records:** `materials/icbm152/original/icbm152_ext55_model_asym_2020_nifti.zip`; `materials/icbm152/selected/mni_icbm152_t1_tal_nlin_asym_55_ext.nii`; `materials/icbm152/license/COPYING`; `materials/provenance/ICBM152_PROVENANCE.md`; `release/neuropen_reference_head_v1/LICENSES/ICBM152_COPYING`.
- **Recorded hashes:** archive `17e46569d109c12e46745f75c4d950ceb386a97dd98cde6e83c0189837886841`; bundled `COPYING` `136665f560a6f60a0dc8a4d9dd752515e6d72bf1050ed9af83c318437fcec121`.

The exact text from the local `COPYING` file is retained here:

> Copyright (C) 1993-2020 Louis Collins, McConnell Brain
> Imaging Centre, Montreal Neurological Institute, McGill University.
> Permission to use, copy, modify, and distribute this software and
> its documentation for any purpose and without fee is hereby granted,
> provided that the above copyright notice appear in all copies.  The
> authors and McGill University make no representations about the
> suitability of this software for any purpose.  It is provided "as
> is" without express or implied warranty.  The authors are not
> responsible for any data loss, equipment damage, property loss, or
> injury to subjects or patients resulting from the use or misuse of
> this software package.

### RWTH adult head-and-torso scan — lower-form shape guidance

- **Source / authors:** Hark Simon Braren and Janina Fels (2020), *A High-Resolution Individual 3D Adult Head and Torso Model for HRTF Simulation and Validation: 3D Data*, RWTH Aachen University, DOI [10.18154/RWTH-2020-06760](https://doi.org/10.18154/RWTH-2020-06760).
- **Official source:** [RWTH Publications record](https://publications.rwth-aachen.de/record/793260), which identifies the STL, technical report, authors, DOI, and CC BY 4.0.
- **Use:** A registered cross-section from the RWTH model served as general shape guidance. No RWTH donor triangles were transferred into the final mesh; this is reference-guided support, not a direct RWTH surface copy.
- **License / attribution:** CC BY 4.0. Attribute Braren and Fels (2020), the dataset title, RWTH Aachen University, and DOI; link the [license](https://creativecommons.org/licenses/by/4.0/) and identify changes. The source STL was reoriented/registered for cross-section comparison; no source faces were copied.
- **Local records:** `materials/rwth_head_torso/original/3DModel.stl`; `materials/rwth_head_torso/docs/TechnicalReport_3DModel.pdf`; `materials/rwth_head_torso/license/CC-BY-4.0-legalcode.txt`; `materials/provenance/RWTH_HEAD_TORSO_PROVENANCE.md`; `release/neuropen_reference_head_v1/LICENSES/RWTH_CC-BY-4.0-legalcode.txt`.
- **Attribution:** Braren, H. S. and Fels, J. (2020), *A High-Resolution Individual 3D Adult Head and Torso Model for HRTF Simulation and Validation: 3D Data*, RWTH Aachen University, DOI: 10.18154/RWTH-2020-06760, CC BY 4.0. Changes: reoriented and registered for cross-section shape guidance; no donor triangles transferred.
- **Provenance limitation:** The publisher-hosted binary could not be fetched in the recorded environment; the local source identity was checked against the authors’ reported mesh counts and a source mirror. See the local provenance record.

### EEG position labels — `eeg_positions` (MIT)

- **Source / owner:** `eeg_positions` developers; repository maintained at [github.com/sappelhoff/eeg_positions](https://github.com/sappelhoff/eeg_positions), Zenodo record [10.5281/zenodo.3718568](https://doi.org/10.5281/zenodo.3718568).
- **Use:** Coordinate-free 10-20, 10-10, and 10-5 label inventories are retained as source-scoped label references and cross-checks. Their XYZ columns are not used as Neuropen coordinates. The selected 10-5 release set is separately scoped and excludes non-recording marks, fiducials, and face-boundary labels.
- **License / notice:** MIT License. The copied license text permits use, modification, distribution, and sale subject to retaining its copyright and permission notice and its warranty/liability disclaimer. Required notice: “Copyright (c) 2018 eeg_positions developers”.
- **Local records:** `materials/10x/label_sets/10-20_eeg_positions_raw_label_inventory.tsv`; `materials/10x/label_sets/10-10_eeg_positions_raw_label_inventory.tsv`; `materials/10x/label_sets/10-5_eeg_positions_raw_label_inventory.tsv`; `materials/10x/sources/EEG_POSITIONS_LICENSE.txt`; `materials/10x/SOURCE_MANIFEST.json`.

### ACNS 10-10 nomenclature — names-only extraction

- **Source / authors:** Acharya JN, Hani A, Cheek J, Thirumala P, Tsuchida TN (2016), “ACNS Guideline 2: Guidelines for Standard Electrode Position Nomenclature,” *Journal of Clinical Neurophysiology* 33:308–311, DOI [10.1097/WNP.0000000000000316](https://doi.org/10.1097/WNP.0000000000000316). [ACNS guideline index](https://www.acns.org/practice/guidelines) · [Official paper](https://www.acns.org/UserFiles/file/Guideline2-GuidelinesforStandardElectrodePositionNomenclature_v1.pdf).
- **Use:** Nomenclature reference and source for the 71-name 10-10 label inventory. The repository contains a names-only transcription of Figure 1 labels; it does not contain the figure image, its pixels, or source XYZ coordinates.
- **Terms / local records:** The project research record states that the paper is copyrighted and warns against unauthorized reproduction. `materials/10x/label_sets/10-10_acns2016_fig1_71.tsv` is the local extraction; `materials/10x/SOURCE_MANIFEST.json` records its scope. No separate permission for redistribution of the transcription is recorded here.

## Research and QA only — not incorporated into final model geometry

### HUTUBS head meshes

- **Source / authors:** Fabian Brinkmann, Manoj Dinakaran, Robert Pelzer, Jan Joschka Wohlgemuth, Fabian Seipel, Daniel Voss, Peter Grosche, and Stefan Weinzierl, *The HUTUBS head-related transfer function (HRTF) database* (2019), TU Berlin Audio Communication Group, DOI [10.14279/depositonce-8487](https://doi.org/10.14279/depositonce-8487). [Canonical DepositOnce record](https://depositonce.tu-berlin.de/items/dc2a3076-a291-417e-97f0-7697e332c960) · [SOFAcoustics dataset index](https://sofacoustics.org/data/database/hutubs/).
- **Use:** PP2 and comparison head meshes were inspected and used in rejected local ear-patch experiments. No HUTUBS donor triangles are present in the final model.
- **Dataset terms:** The HUTUBS documentation says the data are provided under CC BY 4.0; the local documentation also requests citation. Attribute the database and its authors, link CC BY 4.0, and indicate changes if adapting data. The archived DepositOnce `license.txt` is a repository deposit/publishing agreement, not the downstream data license.
- **Local records:** `materials/hutubs/selected/`; `materials/hutubs/docs/Documentation.pdf`; `materials/hutubs/docs/AntrhopometricMeasures.pdf`; `materials/hutubs/license/CC-BY-4.0.txt`; `materials/hutubs/license/DepositOnce_license.txt`; `materials/provenance/HUTUBS_PROVENANCE.md`.
- **Separate article-copy issue:** `materials/hutubs/docs/brinkmann_etal_2019.pdf` is an author-accepted manuscript whose first page says it is protected by copyright and that other uses require rights-holder permission. A separate public redistribution grant for this local article PDF is not recorded. This is distinct from the HUTUBS dataset’s CC BY terms.

### HSRD-100 human scans

- **Source / owner:** Digital Reality Lab, *HSRD-100: 100 High-Quality 3D Human Scans Dataset from HumanScanRepository*. [Dataset repository](https://huggingface.co/datasets/digitalrealitylab/HSRD-100); local snapshot `9cc5e9c138dd310dc88c95c80e5db0a3ecb7971a`.
- **Use:** A selected LOD0 scan and previews were inspected for research and QA. No HSRD geometry contributed to the final model.
- **License / attribution:** The dataset card declares CC BY 4.0. Attribute Digital Reality Lab and the dataset, link CC BY 4.0, and identify adaptations if any. The same dataset card separately says the data are not intended for medical applications and excludes biometric identification and surveillance. That statement is distinct from the CC BY license; the project’s compatibility with the medical-application statement is unresolved.
- **Local records:** `materials/hsrd100/original/`; `materials/hsrd100/selected/`; `materials/hsrd100/docs/`; `materials/hsrd100/license/CC-BY-4.0.html`; `materials/provenance/HSRD100_PROVENANCE.md`.

### openSAHE precomputed atlas mask

- **Source / authors:** Fernando S. Moura, Roberto G. Beraldo, Leonardo A. Ferreira, and Samuli Siltanen, *openSAHE: Open Source Statistical Anatomical Atlas of the Human head for Electrophysiology Applications (precomputed atlases)*, v1.0 (2021), DOI [10.5281/zenodo.5559624](https://doi.org/10.5281/zenodo.5559624). [Zenodo record](https://zenodo.org/records/5559624).
- **Use:** The mask and derived scalp candidates were used in earlier source comparison and QC. They were not promoted to the final geometry; the final head is derived from ICBM152 Extended 2020.
- **License / attribution:** The Zenodo record declares CC BY 4.0. Attribute the authors and dataset, link the license, and identify changes when sharing adaptations.
- **Local records:** `materials/opensahe/selected/Atlas_conductivity_freq_100_RFact_111_Mask.nii`; `materials/opensahe/docs/zenodo_record_5559624.json`; `materials/opensahe/license/CC-BY-4.0.txt`; `materials/provenance/OPENSAHE_PROVENANCE.md`.

## Literature and software references — nomenclature, method, and QA

These references informed nomenclature, measurement context, or independent method checks. Except for the ACNS names-only list described above, no paper figure or article text was copied into the 10-X label/material bundle.

- Jasper HH (1958), original 10-20 proposal, DOI [10.1016/0013-4694(58)90053-1](https://doi.org/10.1016/0013-4694(58)90053-1): citation only; no paper or figure copied.
- Klem GH, Lüders HO, Jasper HH, Elger C (1999), IFCN 10-20 description, [PubMed 10590970](https://pubmed.ncbi.nlm.nih.gov/10590970/): citation and 19-site scope reference; no article copied.
- Chatrian GE, Lettich E, Nelson PL (1985), historical 10% system, DOI [10.1080/00029238.1985.11080163](https://doi.org/10.1080/00029238.1985.11080163): citation only.
- Oostenveld R and Praamstra P (2001), original 10-5 proposal, DOI [10.1016/S1388-2457(00)00527-7](https://doi.org/10.1016/S1388-2457(00)00527-7): contour/nomenclature reference; citation only.
- Seeck M et al. (2017), IFCN standardized array, DOI [10.1016/j.clinph.2017.06.254](https://doi.org/10.1016/j.clinph.2017.06.254), and Peltola ME et al. (2023), IFCN–ILAE routine/sleep EEG standards, [open article](https://pmc.ncbi.nlm.nih.gov/articles/PMC10006292/): clinical-array context; citation only.
- Jurcak V, Tsuzuki D, Dan I (2007), 10/20, 10/10, and 10/5 systems revisited, DOI [10.1016/j.neuroimage.2006.09.024](https://doi.org/10.1016/j.neuroimage.2006.09.024): citation only.
- Giacometti P, Perdue KL, Diamond SG (2014), mesh-based high-density scalp-coordinate method, [PubMed 24769168](https://pubmed.ncbi.nlm.nih.gov/24769168/): independent computational precedent; the project does not claim to reproduce its exact algorithm.
- FieldTrip electrode-localization tutorial, [official documentation](https://www.fieldtriptoolbox.org/tutorial/source/electrode/) and [repository](https://github.com/fieldtrip/fieldtrip): implementation cross-check only. No FieldTrip code or position file is present in the final release. The prior project research record identifies the repository code/data as GPL-3.0; no FieldTrip license is applied to Neuropen assets.
- MNI source-page snapshots at `materials/icbm152/docs/icbm152_2020_source_index.html` and `materials/icbm152/docs/mcgill_icbm152_overview.html` were retained for source/metadata review, not copied into the model. The exact atlas archive’s bundled `COPYING`, rather than the older overview page, is the recorded basis for the ICBM-derived mesh notice.

## Checked and not found

No VHP (Visible Human Project) mesh, image, license file, or provenance entry was found in the current source manifest, source records, or `materials/` tree. No VHP data use or geometry contribution is documented for the final model.

## Project-created reference artwork

The three schematic SVGs under `materials/10x/figures/` are recorded as project-created, illustrative diagrams released under CC0 1.0; they were not traced from source figures and are not geometry. See `materials/10x/figures/README.md` and `materials/10x/SOURCE_MANIFEST.json`.

## Items still requiring a project decision before public repository distribution

- **Project-owned assets:** This checkout contains no selected license for the Neuropen-owned mesh, coordinates, markers, renders, or project documentation. The README intentionally leaves a placeholder; a third-party source license does not grant a project-wide license to these assets.
- **HSRD-100 research files:** The data card declares CC BY 4.0 but also says the dataset is not intended for medical applications. Compatibility with this EEG reference-head project is not resolved. The raw scan and related research files remain under `materials/hsrd100/`, outside the final release package.
- **HUTUBS article PDF:** Redistribution rights for `materials/hutubs/docs/brinkmann_etal_2019.pdf` are not established by the separate CC BY license for HUTUBS data.
- **ACNS-derived 10-10 label list:** The source guideline warns against unauthorized reproduction. The local 71-name transcription contains no figure pixels or coordinates, but no separate permission for distributing that transcription is recorded.
- **Archived MNI webpages:** `materials/icbm152/docs/icbm152_2020_source_index.html` and `materials/icbm152/docs/mcgill_icbm152_overview.html` are local source-page captures. No page-specific redistribution grant is recorded for these HTML copies; they are not part of the final model release. Review them separately or rely on the linked official pages if publishing the wider research checkout.

These open items do not change the source attribution or coordinate provenance. They mean the current notices record is not evidence that every file in the wider research checkout has been cleared for public redistribution.
