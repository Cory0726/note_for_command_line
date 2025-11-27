# note_for_command_line
My note for Commnad-line interface.

- [git](#git)
- [Anaconda](#anaconda)
- [Linux](#linux)
- [Nvidia](#nvidia)

## git
### [git install](https://git-scm.com/install/windows)
```bash
git --version

git clone <your_repo_url>
git remote -v
git remote add origin <your_git_url>

git status
git branch
git log

git pull origin <your_branch>
git pull origin <your_branch> --rebase
git add .
git add <your_file_1> <your_file_2>

git commit -m "<your_message>"
git rm --cached <your_file>
git push origin <your_branch>

git fetch origin
git reset --hard origin/your_branch
git clean -fd
```
---

## [Anaconda](https://anaconda.org/)
### [Download Anaconda](https://www.anaconda.com/download/success)
### Command
```bash
# Environment
conda env list
conda activate <your_env_name>
conda deactivate

conda export --file environment.yml
conda env create -f environment.yml
conda env update --file environment.yml --prune
conda env remove -n <your_env_name>

# Package
conda install <your_package_name>
conda remove <your_package_name>
conda list
conda list <your_keyword>
```
### Issue
#### Error while loading conda entry point: conda-libmamba-solver (module 'libmambapy' has no attribute 'QueryFormat')
- 開**Anaconda Prompt**
```bash
conda update conda
conda update conda-libmamba-solver
```
---

## Linux
```bash
# CPU Info
lscpu

# apt
sudo apt update
sudo apt upgrade
```
## Nvidia
```commandline
nvidia-smi
```
