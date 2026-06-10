# From Logical to Concrete: OpenSCENARIO 2.0–Driven Scenario Extraction from Naturalistic Driving Data

> Accepted for publication at the IEEE Intelligent Transportation Systems Conference (ITSC)

## Overview

This repository contains the research paper resulting from my Master's thesis, accepted for publication at the IEEE Intelligent Transportation Systems Conference (ITSC).

The work presents a formal, specification-driven pipeline for extracting concrete traffic scenarios from large-scale naturalistic driving datasets using ASAM OpenSCENARIO 2.0. Instead of relying on heuristic tagging, threshold-based filtering, or machine learning classifiers, the proposed approach directly evaluates formal scenario semantics over real-world vehicle trajectories.

## Abstract

Scenario-based virtual validation relies on logical scenario specifications that define classes of traffic situations through parameterized descriptions. These logical scenarios are typically sampled to generate finite sets of executable, concrete simulation instances. However, existing approaches typically do not directly leverage such formal logical specifications to extract corresponding concrete instances from naturalistic driving datasets (NDD).

This paper presents a formal scenario extraction pipeline that uses OpenSCENARIO 2.0 logical descriptions as constraint-generating specifications for data-driven scenario identification. From each logical scenario, compositional and temporally anchored constraints are derived and evaluated over reconstructed road-aligned actor traces.

To enable scalable and semantically consistent filtering, the method reconstructs lane topology from NDD map primitives, aggregates topology-invariant road segments, and establishes an OpenDRIVE-compatible lane indexing scheme for relational reasoning.

The approach is evaluated on the Waymo Open Motion Dataset for multiple ADAS-relevant scenario classes and demonstrates scalable search-space reduction, deterministic semantic constraint enforcement, and realistic parameter domains derived directly from real-world driving data.

## Key Contributions

* Formal mapping from OpenSCENARIO 2.0 logical scenarios to concrete instances in naturalistic driving datasets
* Deterministic scenario extraction based on scenario semantics rather than learned classifiers
* Reconstruction of lane-level topology and road structure from raw map data
* OpenDRIVE-compatible lane indexing for relational reasoning
* Scalable extraction pipeline for large-scale driving datasets
* Validation using the Waymo Open Motion Dataset

## Results

The methodology was evaluated on three ADAS-relevant scenario types:

| Scenario                                | Extracted Instances |
| --------------------------------------- | ------------------: |
| Cut-In                                  |               9,814 |
| Car-to-Car Rear Braking (CCRb)          |              10,244 |
| Car-to-Pedestrian Nearside Adult (CPNA) |               4,456 |

The extracted scenario instances satisfy all formally defined OpenSCENARIO 2.0 constraints and provide realistic parameter distributions directly derived from real-world traffic behavior.

## Publication

**Title**

*From Logical to Concrete: OpenSCENARIO 2.0–Driven Scenario Extraction from Naturalistic Driving Data*

**Authors**

Patrick Kasten, Dörte Waldöstl, Ahmed Rida Sekkat, Oliver Sawade, Elmar Matthes

**Conference**

IEEE Intelligent Transportation Systems Conference (ITSC)

**Status**

Accepted for publication

DOI and citation information will be added once the final publication becomes available.

## Repository Contents

```text
.
├── paper.pdf
└── README.md
```

## Research Context

This research was conducted as part of my Master's thesis at IAV GmbH in Berlin, Germany, focusing on scenario-based validation for automated driving systems and the integration of formal scenario descriptions with large-scale naturalistic driving data.

## Contact

Patrick Kasten

GitHub: https://github.com/Patrone411

LinkedIn: [www.linkedin.com/in/patrick-kasten](http://www.linkedin.com/in/patrick-kasten)

## License

This repository is intended for academic and professional reference.

The final published version of the paper is subject to IEEE copyright and publication policies.
