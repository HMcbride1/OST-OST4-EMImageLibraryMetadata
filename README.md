This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project code is provided on an ‘as is’ basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
# Fisheries EM Image Library Metadata Best Practices

## Overview
This repository serves as a collaborative workspace for developing metadata best practices and common export schemas for NOAA Fisheries annotated commercial fisheries species image libraries. 

Rather than dictating how individual projects structure their internal annotation workflows, this effort focuses on defining a standardized schema for **final data exports**. Establishing common export standards allows image libraries across regions to be queried effectively, shared efficiently, and leveraged for multi-model machine learning and AI development.

## Participating Projects & Teams
This initiative brings together leads and developers across two primary NOAA Fisheries AI/ML commercial fisheries image library efforts:
* **NEFSC / Bigelow EM Image Library & Model Sharing Project** (NEFSC & CVision AI)
* **Alaska Fisheries AI/ML Project** (AFSC / AKRO)
* **Coordination:** NOAA Fisheries Office of Science and Technology (OST)

## Scope & Core Standardization Areas
Our initial phase of standardization focuses on two core components:

1. **Operational Metadata**
   Standardizing external parameters generated alongside the video feed, including temporal, spatial, and gear-specific data.
2. **Core Ground Truth Annotations**
   Establishing consistent formatting for key biological labels so libraries can be queried across projects—specifically focusing on **verified species identification** and **length measurements** (where applicable).

## Metadata Framework Approach
After evaluating existing frameworks (including EVERYFISH COCO and netCDF4), the working group selected **Darwin Core** as the primary foundation due to its strong biological data structure. 

* **Workflow Flexibility:** Teams maintain their own internal annotation pipelines while aligning on standardized Darwin Core export mappings.
* **Key Decision Points:** Using representative operational metadata exports as a baseline to align on field names, units, and areas requiring schema flexibility.

## Repository Structure
* `README.md` — Project overview, scope, and working group guidelines.
* `resources/` — Reference schemas, sample Darwin Core exports, field mapping drafts, and supporting documentation.

## Current Objectives & Next Steps
* Share representative operational metadata exports (using the Bigelow EM Image Library project as an initial baseline).
* Review and align on standardized field names, units, and Darwin Core mappings.
* Identify where schema flexibility is needed to accommodate regional operational differences.
