---
title: 'QXTools: A Julia framework for distributed quantum circuit simulation'
tags:
  - Julia
  - Qunatum computing
  - Simulation
  - Tensor networks
authors:
  - name: Momme Allalen
    affiliation: 1
  - name: David Brayford
    affiliation: 1
  - name: John Brennan
    affiliation: 2
  - name: Myles Doyle
    affiliation: 2
  - name: Kenneth Hanley
    affiliation: 2
  - name: Luigi Iapichino
    affiliation: 2
  - name: Niall Moran^[corresponding author]
    orcid: 0000-0002-2619-5040
    affiliation: 2
#    affiliation: "1, 2" # (Multiple affiliations must be quoted)
  - name: Lee O’Riordan
    affiliation: 2
affiliations:
 - name: Leibniz Supercomputing Centre
   index: 1
 - name: Irish Centre for High-End Computing, Ireland
   index: 2
date: 12 August 2021
bibliography: paper.bib

---

# Summary

QXTools is a framework for simulating quantum circuits using tensor network methods.
It is designed to run on large distributed compute clusters and supports GPU
accelerators. The simulation workflow is broken down into a number of stages, each
of which is managed by a special purpose package that can be used independently or
as part of the QXTools framework. A domain specific language (DSL) is used to
represent the simulation as a set of tensor network operations.
This separates the high level index accounting and contraction planning from the
low level implementation of the tensor network operations and makes it easier to
support new hardware and network architectures.

# Statement of need

As quantum processing devices continue to scale and the algorithms and experiments
being run on them grow in complexity, simuulations of these systems become much
more computationally demanding. To reduce the turn around time and
allow larger systems to be simulated it is necessary to move beyond single workstations
and use distributed compute clusters. QXTools provides a flexible, extensible open source
framework for performing these simulations. The use of Julialang makes it easy for the code
to be understood, modified and extended while not sacrificing performance compared to
compiled languages.

<!-- # Citations

Citations to entries in paper.bib should be in
[rMarkdown](http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)
format.

If you want to cite a software repository URL (e.g. something on GitHub without a preferred
citation) then you can do it with the example BibTeX entry below for @fidgit.

For a quick reference, the following citation commands can be used:
- `@author:2001`  ->  "Author et al. (2001)"
- `[@author:2001]` -> "(Author et al., 2001)"
- `[@author1:2001; @author2:2001]` -> "(Author1 et al., 2001; Author2 et al., 2002)"

# Figures

Figures can be included like this:
![Caption for example figure.\label{fig:example}](figure.png)
and referenced from text using \autoref{fig:example}.

Figure sizes can be customized by adding an optional second parameter:
![Caption for example figure.](figure.png){ width=20% } -->

# Acknowledgements

This work was financially supported by the PRACE project funded in part by the EU’s
Horizon 2020 Research and Innovation programme (2014-2020) under grant agreement 823767.

# References