# Awesome Bash Scripts

This repository contains a collection of bash shell scripts aimed at boosting productivity during development tasks. These scripts are located in the `bin` directory.

- `git-amend`: amend the latest commit without changing the commit message.
- `git-commit-branch-name`: generates a commit message based on the current branch name, following a specific prefix convention. It then commits the changes with this generated message.
  - E.g `$ git-commit-branch-name`
  - Branch name and commit message examples
    - `feature/add-new-feature` -> `feat: add new feature`
    - `refactor/update-algorithm` -> `refactor: update algorithm`
    - `fix/issue123` -> `fix: resolve issue123`
    - `chore/update-dependencies` -> `chore: update dependencies`
    - `docs/update-readme` -> `docs: update readme`
- `git-delete-merged-branches`: delete all local branches that have been merged except for the `main`, `master`, or `develop` branches.
  - E.g `$ git-delete-merged-branches`
- `git-tag-and-push`: delete a Git tag both locally and remotely, and then reapply the tag to the current commit, forcing the update in the remote repository.
  - E.g `$ git-tag-and-push v1.0.0`
- `ts-index-generate`: generate an index file for TypeScript modules. It iterates over all TypeScript files in a directory (excluding index.ts), and appends export statements for each file to the specified index file.
  - E.g `$ ts-index-generate path/to/your/index.ts`

## Installation

To get started, you need to clone this repository to your local machine. Open your terminal and run the following command:

```bash
$ git clone git@github.com:10xDeveloperTW/bash.git
```

## Usage

Once you have cloned the repository, you can use these scripts in a couple of ways:

### Option 1: Direct Execution

You can execute the scripts directly from the repository by navigating to the bin directory and running them. For example:

```bash
bash/bin/ts-index-generate
```

### Option 2: Adding Scripts to Your PATH

To make these scripts globally accessible from anywhere in your terminal, you can add the bin directory to your `PATH` environment variable.

#### Step 1: Add the `bin` Directory to Your PATH

Open your shell configuration file (e.g., `~/.bashrc`, `~/.bash_profile`, `~/.zshrc`, etc.) in a text editor, and add the following line at the end:

```bash
export PATH="/path/to/bash/bin:$PATH"
```

Replace /path/to/bash with the actual path to the cloned repository.

#### Step 2: Source the Shell Configuration File

Save the changes to your shell configuration file and then source it to apply the changes immediately:

```bash
$ source ~/.bashrc  # or ~/.bash_profile, ~/.zshrc, etc.
```

Now you should be able to execute any script from anywhere in your terminal by simply typing its name, like so:

```bash
ts-index-generate
```
