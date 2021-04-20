# MInChI: Mixtures InChI

## Introduction

TBD

## Specification

* Specification documentation: [DRAFT](https://docs.google.com/document/d/1X3Mj1iyEPVBfQhDxn8r6ClKsGqhhiKxzuNC9FuTip84/edit?usp=sharing)
* Pilot implementation reference: [Capturing mixture composition: an open machine-readable format for representing mixed substances](https://doi.org/10.1186/s13321-019-0357-4), A.M. Clark, L.R. McEwen, P. Gedeck, B.A. Bunin, *Journal of Cheminforamtics 2019* 

## Validation Data

A preliminary collection of mixtures has been selected as a candidate for the MInChI validation set: ca. 150 mixtures were taken from a large corpus of marked up catalog data and clustered based on branch structure and component characteristics (presence of structure, unit types, range format, etc.). Most of the possible edge cases for MInChI notation should be found to occur in at least one example. They are represented using the _Mixfile_ format. The list needs to be curated, and then the MInChI notation for each of them created programmatically and then checked.

* [validation/validation.json](validation/validation.json)

## Links

* Mixture Editor: <https://github.com/cdd/mixtures>
* MInChI Live Demo: <http://molmatinf.com/minchidemo> and its source on [GitHub](https://github.com/IUPAC/MInChI_demo)
