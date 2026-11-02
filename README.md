
# ABJM SageMath Subsector Classification

This repository contains the SageMath code developed as part of my master's thesis on **Spin Matrix Theory and ABJM**.

The program is used to identify and classify possible near-BPS decoupled subsectors of ABJM theory.

## What the code does

The code uses SageMath's polyhedron functionality to find combinations of Cartan charges satisfying the free BPS bound

\[
\Delta_0 \geq J.
\]

For each allowed combination of charges, the surviving letters are those satisfying \(\Delta_0-J=0\).

The program allows us to:

- Construct the allowed region using exact rational arithmetic.
- Identify candidate subsectors from the faces of the resulting polyhedron.
- Require both bifundamental and anti-bifundamental letters, consistent with the alternating structure of ABJM gauge-invariant operators.
- Identify equivalent subsectors using SU(4) R-symmetry transformations, spin-flips, and dagger-swaps.
- Work with predefined Cartan bases or introduce new ones.

Using the procedure described in the thesis, we find **214 decoupled subsectors**, which reduce to **10 inequivalent types** after accounting for the relevant symmetries.

## Requirements

The code is contained in a Jupyter Notebook (`.ipynb`) and uses SageMath functionality.

To execute it, you need:

- [SageMath](https://www.sagemath.org/)
- Jupyter Notebook with a SageMath kernel

The notebook cannot be run using ordinary Python alone.

For development on Windows, SageMath was used through the Windows Subsystem for Linux (WSL).

## How to run

1. Download the notebook from this repository.
2. Open it in Jupyter Notebook with a SageMath kernel.
3. Run the notebook cells in order.
4. Adjust the Cartan basis and symmetry options to explore different subsectors.

GitHub also provides a static preview of the notebook, so the code and any saved outputs can be viewed directly in the browser.

## Thesis reference

This code accompanies my master's thesis on Spin Matrix Theory and its extension to ABJM theory (2026).

The mathematical procedure and classification results are discussed in the section *Identifying decoupled sectors of ABJM with SageMath*. Further information about the implementation is provided in the appendix *SageMath Python code*.
