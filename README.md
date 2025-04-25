# SoftwareStacks

## Purpose

This repository serves as a central documentation hub for the creation and management of software stacks designed for data-intensive applications, especially in the life sciences. It aims to support users in building reproducible and portable environments based on trusted resources.

## Available Resources
- [bioconda-recipes](https://github.com/deKCD/bioconda-recipes):
Conda recipes for bioinformatics software packages.
- [multi-package-containers](https://github.com/deKCD/multi-package-containers):
Docker containers bundling multiple conda packages (also known as “mulled containers”).
- [deNBI/resenvs](https://github.com/deNBI/resenvs):
Guidelines and resources for creating virtual machine (VM) images tailored for reproducible computational environments.

## How to Create Your Own Software Stack
1. Choose required software packages:
  - Browse the [bioconda](https://bioconda.github.io/) website or the [bioconda-recipes](https://github.com/deKCD/bioconda-recipes) repository to find relevant packages.
2. Create a Conda environment:
  - Define an environment.yml file listing the packages and versions you want to include.
3. Build a container:
  - Use the [multi-package-containers](https://github.com/deKCD/multi-package-containers) repository as a starting point for creating a Docker container that encapsulates your conda environment.
4. (Optional) Create a VM image:
  - Follow the instructions in the [deNBI/resenvs](https://github.com/deNBI/resenvs) repository to build a virtual machine image with your stack.

## Example Structure for a New Stack
```bash
my-software-stack/
├── environment.yml
├── Dockerfile
├── README.md
└── tests/
    └── test_script.sh
```
