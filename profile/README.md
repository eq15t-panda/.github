# PANDA

**Photon-Atom Non-linearities and Deterministic Applications via arrays**

PANDA is a project aiming to build the foundation for a scalable photonic quantum computer using neutral atoms. By leveraging collective effects and deterministic photon-photon interactions, PANDA addresses the core challenges of quantum information processing (QIP) with photons.

The consortium includes:
- **Sorbonne Université** (coordinator) — France
- **PASQAL** — France
- **Institut d'Optique**, Saclay — France
- **ICFO** (The Institute of Photonic Sciences) — Spain
- **Pixel Photonics GmbH** — Germany

---

## About this GitHub organization

This organization hosts the software developed by the PANDA collaboration at Sorbonne Université, covering both experimental control/data acquisition and theoretical/numerical optimization work supporting the project's cavity QED and non-linear optics efforts.

### Main Repositories

#### [`PANDAManager`](https://github.com/eq15t-panda/PANDAManager)
A small Python-based laboratory data-acquisition and plotting project (notebooks + helpers) used to control instruments, acquire datasets, and produce reproducible plots.

- Instrument control: power meters, oscilloscopes, temperature controllers, etc.
- Jupyter notebooks for interactive acquisition and plotting
- Instrument configuration files (JSON)
- Raw/processed data storage
- Utility modules implementing common acquisition and plotting helpers

#### [`PANDASimulation`](https://github.com/eq15t-panda/PANDASimulation)
Scripts developed to find the optimal parameters for a chosen non-linear crystal and optical cavity geometry.

- Focused solely on the practical aspect of parameter optimization
- Does not include literature review or theoretical background
- Covers cavity design (e.g. bow-tie geometries), phase-matching, and focusing optimization for second-harmonic generation

---

## Getting started

Each repository contains its own README with setup instructions, dependencies, and usage examples. Please refer to the individual repos for details.

### General information

Required python `>= 3.8` and `pip`

```
pip install -r requirements.txt
```

### Using Pycharm

If you are using Pycharm follow these simple steps:

1. On **GitHub**, click the button <span style="color:lime;"><> Code</span> and copy the link
2. On **Pycharm**, go to `Git > Clone`
3. Paste the url of the **GitHub** repository you just copied and click clone.
4. You can now access the files. The GUI should automatically ask you if you want to download the requirements

### Using Spyder

#### How to clone a repository in Spyder?

Tutorial was found at [this link](https://github.com/spyder-ide/spyder/issues/17271#issuecomment-1031753490).

You need to open a system terminal, go to the directory you want to clone and do `git clone your-repo-here.git`, then you 
can open Spyder and either create a new project in the directory where you cloned your repository, or just open in the 
files pane the directory where you cloned the repository

#### How to sync a Spyder folder with GitHub?

To sync your folder you need to use git commands, https://education.github.com/git-cheat-sheet-education.pdf, normally 
you will have two most use cases that are syncing with your remote repo and publishing your changes to the remote repo.
This has to be done in a system terminal as well.

- Exploring changes: `git fetch`
- Sync remote changes to local repository: `git pull`
- To publish changes, first create a commit with a description and then publish them: 
```
git add -A 
git commit -m "Description of the changes"
git push
```


## Contributing

This is an active research project. Issues and pull requests from consortium members are welcome — please open an issue to discuss significant changes before submitting a PR.

## Contact

For questions about the PANDA project, please reach out to the active developers of each repo.

## License

MIT License

Copyright (c) [2026] [William GENETELLI]
