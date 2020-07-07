# intake-latcat

This is an [intake](https://intake.readthedocs.io/en/latest)
data source for accelerator lattice catalogs where the lattice files are availble in various formats (currently restricted to [MADX](https://mad.web.cern.ch/mad/), [Elegant](https://ops.aps.anl.gov/elegant.html) and [LatticeJson](https://www.github.com/nobeam/latticejson)).

These catalogs are designed to be a standardized format for describing metadata and access information datasets on the available lattices.

This project provides an opinionated way for users to load datasets from these catalogs into the scientific Python ecosystem.

At the moment it loads LatticesJson files into dictionaries, MADX files into strings, Elegant files into strings and Twiss files into Pandas dataframes. When Twiss files are loaded basic plots of Beta functions and Dispersion are also provided, to allow users to quickly visualize the basic standard lattice functions. At a latter stage accelerator layouts will be provided.

Future formats could include plain JSON, Parquet, OPA, AT,...

## Requirements
```
intake >= 0.4.4
```
