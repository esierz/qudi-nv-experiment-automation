# qudi-iqo-modules
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)

---
A collection of qudi measurement modules originally developed for experiments on color centers in 
semiconductor materials.



## Installation
For installation instructions please refer to our
[iqo-modules installation guide](https://github.com/Ulm-IQO/qudi-iqo-modules/blob/main/docs/installation_guide.md).


## More information
The best starting point for further researching the qudi documentation is the [readme file](https://github.com/Ulm-IQO/qudi-core) of the qudi-core repo.

## Forum
For questions concerning qudi or the iqo-modules, there is a [forum](https://github.com/Ulm-IQO/qudi-core/discussions) to discuss with the qudi community. Feel free to ask!
If you found a bug and located it already, please note GitHub's [issue tracking](https://github.com/Ulm-IQO/qudi-iqo-modules/issues) feature.

## Copyright
Check [AUTHORS.md](AUTHORS.md) for a list of authors and the git history for their individual
contributions.

---

## Updating from Upstream

This repository is a fork of the official  
[qudi-iqo-modules](https://github.com/Ulm-IQO/qudi-iqo-modules) repository.

We use two main branches:

- `main` – Clean mirror of the upstream repository  
- `lab-main` – Lab branch containing all custom modifications  

### Updating `main` from upstream

When the upstream repository is updated, pull changes into `main`:

```bash
git checkout main
git fetch upstream
git merge upstream/main
git push origin main
````

This keeps your `main` branch aligned with the original project.

### Updating `lab-main` from `main`

Once `main` is updated, merge those changes into your lab branch:

```bash
git checkout lab-main
git merge main
git push origin lab-main
```

Finally, resolve conflicts.

### Update Flow Summary

```text
upstream/main → main → lab-main
```

* `main` tracks the original project
* `lab-main` includes all lab-specific changes
* Always update `main` before merging into `lab-main`