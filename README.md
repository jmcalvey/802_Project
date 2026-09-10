# SEE-Segment Genetic Processing Replacement

## Project Overview

This project focuses on getting the existing [SEE-Segment](https://github.com/see-insight/see-segment) image segmentation software running reliably and then modifying its genetic processing component.

The first phase of the project will focus on understanding the existing SEE-Segment workflow, setting up the required software environment, reproducing the existing implementation, and working through any dependency, compatibility, or runtime issues that prevent the software from functioning as intended.

Once a working baseline has been established, the primary goal will be to replace the current genetic processing library with an alternative genetic processing library (possibly making it toggleable between the two). The modified implementation will then be compared with the original to determine whether the replacement maintains the expected functionality and segmentation behavior.

## Research Question

Can the genetic processing component of SEE-Segment be replaced with an alternative genetic processing library while maintaining the functionality and segmentation performance of the original workflow?

## Project Goals

The major goals of this project are:

1. Establish a reproducible environment for running SEE-Segment.
2. Identify and resolve issues preventing the existing software from running correctly.
3. Establish a working baseline implementation of SEE-Segment.
4. Identify the interface between SEE-Segment and its current genetic processing library.
5. Replace the current genetic processing library with an alternative implementation.
6. Test and compare the original and modified workflows.

## Project Workflow

The planned workflow is:

```text
SEE-Segment
    |
    v
Set up environment
    |
    v
Run original implementation
    |
    v
Identify and resolve issues
    |
    v
Establish baseline results
    |
    v
Identify genetic processing component
    |
    v
Replace genetic processing library
    |
    v
Test modified implementation
    |
    v
Compare original and modified results
```

## Software Components

The project involves several main components:

* **SEE-Segment** — the existing image segmentation software being studied and modified.
* **Genetic processing library** — the current library used by SEE-Segment for its genetic/evolutionary processing.
* **Replacement genetic processing library** — the alternative library that will be evaluated and integrated.
* **Python environment and dependencies** — the software environment required to reproduce and develop the project.
* **Testing and validation tools** — tools used to verify that the modified implementation behaves as expected.

## Repository Structure

The repository follows the research software project template provided for the course.

```text
.
├── paper/
│   └── proposal.md
├── mypackage/
├── see-segment-master/
├── tests/
├── docs/
├── scripts/
├── environment.yml
├── makefile
└── README.md
```

The repository structure will be updated as the project develops. The see-segment-master folder was imported for easy exploration of the existing software

## Installation and Setup

The project uses the course repository template and its provided environment and Make workflow.

Initialize the project environment with:

```bash
make init
```

Additional dependencies and setup instructions will be documented here as the SEE-Segment software is integrated into the project.

## Basic Workflow

The current development workflow follows the course template:

```bash
make help
make init
make check
make docs
```

The exact SEE-Segment execution workflow will be documented after the baseline implementation has been successfully established.

## Testing and Validation

Testing will occur in two stages.

### Baseline Validation

The original SEE-Segment implementation will first be tested to establish a working baseline. Problems encountered during setup or execution will be documented and resolved where possible.

### Replacement Validation

After replacing the genetic processing library, the modified implementation will be evaluated against the original implementation.

Potential measures of comparison include:

* successful completion of the segmentation workflow
* validity and consistency of segmentation outputs
* segmentation quality where appropriate evaluation data are available
* computational performance
* reproducibility across runs

The specific quantitative metrics and test cases will be finalized after the original implementation has been characterized.

## Project Status

**Milestone 1 — Initial project setup**

The repository has been established from the course research software template. The current focus is on documenting the project, preparing the repository structure, and beginning the process of reproducing the original SEE-Segment implementation.

## Next Step

The immediate next step is to set up and run the original SEE-Segment software, document the issues encountered, and establish a reproducible baseline before modifying the genetic processing component.

## Related Software

This project is based on:

[SEE-Segment](https://github.com/see-insight/see-segment)

The original project will be treated as the baseline implementation for this work.