# Git Contributions Graph

A command-line tool that aggregates commit data from multiple local Git repositories and generates a GitHub-style contributions graph as an HTML file with embedded SVG.

![Screenshot](screenshot.png)

## Overview

This tool scans one or more local Git repositories, aggregates commit counts for each day over a specified period (default: 365 days), and creates an SVG contributions graph similar to GitHub's. The generated graph is embedded in an HTML file, and you can optionally have it opened automatically in your web browser.

## Features

- **Multi-Repository Support:** Aggregate commits from multiple Git repositories.
- **GitHub-Style Graph:** Creates a contributions graph with GitHub-style colors.
- **Customizable Period:** Specify the number of days to include in the graph (default is 365).
- **SVG Output:** The graph is generated as an SVG embedded in an HTML file.
- **Automatic Browser Launch:** Optionally open the generated HTML file in your default web browser.
- **Validation:** Checks that the provided directories are valid Git repositories and ensures that the Git command is installed.

## Installation

Download `git-contrib-graph`, copy it into a directory on your PATH, and make it executable:

```bash
chmod +x git-contrib-graph
```

## Usage

Run the script with one or more paths to your Git repositories:

```bash
git-contrib-graph /path/to/repo1 /path/to/repo2 -o contributions.html --open
```

### Command-Line Options

- `REPO_PATH`: Path(s) to local Git repositories (multiple allowed).
- `-o`, `--output`: Output HTML file name (default: `contributions.html`).
- `-d`, `--days`: Number of days to include in the graph (default: `365`).
- `-a`, `--author`: Author(s) to include in graph (default: all).
- `-w`, `--open`: Automatically open the generated HTML file in your web browser.

## License

This project is licensed under the MIT License.

