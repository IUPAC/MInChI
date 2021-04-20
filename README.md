# MInChI: Mixtures InChI

## Introduction

All chemicals exist as mixtures in practice, and mixed substances represent a significant fraction of chemical catalogs and laboratory stocks. Chemical composition impacts reactivity, unintentionally or designed. Communicating information about composition is critical for conducting safe, effective, and scientifically meaningful chemistry and other laboratory functions. There is a practical need to connect data and information on mixtures and individual components to facilitate analysis on properties, composition, etc. This IUPAC project ([2015-025-4-800](https://iupac.org/project/2015-025-4-800)) describes a method to apply the IUPAC InChI identifier to describe what is definitively known about the chemical composition of a given mixed substance, generating an unambiguous machine-readable linear notation for mixed substances of uniform properties that can resolve to unique components.  

The MInChI notation is tailored for a primary use case to describe what is definitively reported for source components at the time of mixing. The initial phase is focused on components with molecular structures that produce a well defined standard InChI identifier. Separate, discrete components allows for easy association of arbitrary concentrations. Other types of components may be considered for future phases of the project. While the core InChI identifier lends some canonical characteristics to the notation, for most use cases it is not appropriate to assume that two equivalent mixtures will have an identical MInChI description. The definition of a mixture is not a discrete concept as concentrations always have uncertainty associated with them (whether specified or not) and there are frequently unknown components (which may or may not be anticipated).

* Project reports: ([Google Drive](https://drive.google.com/drive/folders/1qGadCch_n0nzkXnLdg6ayxkZMY7G9vim?usp=sharing))

## Specification

* Specification documentation: [DRAFT](https://docs.google.com/document/d/1X3Mj1iyEPVBfQhDxn8r6ClKsGqhhiKxzuNC9FuTip84/edit?usp=sharing)
* Pilot implementation reference: [Capturing mixture composition: an open machine-readable format for representing mixed substances](https://doi.org/10.1186/s13321-019-0357-4), A.M. Clark, L.R. McEwen, P. Gedeck, B.A. Bunin, *Journal of Cheminforamtics 2019* 

## Validation Data

A preliminary collection of mixtures has been selected as a candidate for the MInChI validation set: ca. 150 mixtures were taken from a large corpus of marked up catalog data and clustered based on branch structure and component characteristics (presence of structure, unit types, range format, etc.). Most of the possible edge cases for MInChI notation should be found to occur in at least one example. They are represented using the _Mixfile_ format. The list needs to be curated, and then the MInChI notation for each of them created programmatically and then checked.

* [validation/validation.json](validation/validation.json)

## Links

* Mixture Editor: <https://github.com/cdd/mixtures>
* MInChI Live Demo: <http://molmatinf.com/minchidemo> and its source on [GitHub](https://github.com/IUPAC/MInChI_demo)
