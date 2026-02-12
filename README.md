# Personal Copier Templates
I tend to deploy the same scaffolding over and over even across languages, with some trends including CI, literate programming, VCS, etc, so what could go wrong with a huge template amirite? These depend on [copier](https://github.com/copier-org/copier) to properly build an encapsulated, directory-specific profile for development, easily deployed thanks to [devenv](https://devenv.sh).

---
## Preliminaries
1. Copier installation: Follow the instructions at https://copier.readthedocs.io/en/stable/#installation
2. Devenv installation: Follow the instructions at https://devenv.sh/getting-started#installation
3. Direnv installation: Follow the instructions at https://direnv.net/docs/installation.html#installation

---
## Quick Start
Use Copier to clone this repo.
```bash
copier copy git@github.com:jerivl/copier-templates.git <destination>
```
After the questionaire, you will be prompted on entering the directory to allow a new direnv profile with `direnv allow`. 
```bash
cd <destination>
direnv allow
```
The build will then commence, and depending on how many features you enabled, it may take a while. Thankfully, devenv will cache this environment by default for near instant activations afterwards.

---
Only accepting PRs related to build speed and security. I can't maintain every language or tool, but feel free to fork!
