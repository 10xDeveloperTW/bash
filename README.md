# Awesome Bash Scripts

This repository contains a collection of bash shell scripts aimed at boosting productivity during development tasks. These scripts are located in the `bin` directory.

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
