# Parsons Lab — Quantum Hardware Engineering

**University of Washington · Electrical & Computer Engineering**

We mostly shine lasers and microwaves at atoms and atom-like systems to control their quantum states. We are currently 
focused on neutral-atom quantum computing and spin-defect quantum memories in diamond. This organization holds the code 
behind our work.

The diamond quantum memory project code and our lab forks of ARTIQ and QICK live in the [QT3 organization](https://github.com/qt3uw).

## For lab members

**`main` is protected.** Every change goes through a pull request with one approval. The point is a record of *why* a change was made, not gatekeeping — a one-line PR description is fine.

**Data does not go in git.** Instrument output — `.h5`, `.npy`, `.tdms`, raw scans — belongs in the data store. Git holds the code that produced it. A few hundred MB committed once slows every clone in the lab forever, and removing it means rewriting history.

**Never commit credentials.** Push protection will usually catch it, but a key that reaches history has to be rotated, not just deleted.

**Start new repositories from [`lab-template`](#).** License, `.gitignore`, CI, and citation metadata come pre-configured. Use the template dropdown when you create the repo.

**Naming:** lowercase, hyphen-separated, no dates, no personal names. Add topics — they're the only way to find anything once we have fifty repos.

**Publishing a paper?** Talk to Max before making a repository public. There's a checklist: history audit, license, `CITATION.cff`, then a Zenodo DOI minted from a release tag.

## Contact

mfpars [at] uw [dot] edu · [wp.ece.uw.edu/parsons](https://wp.ece.uw.edu/parsons/)
