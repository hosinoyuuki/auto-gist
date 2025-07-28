# ug - Upload file to GitHub Gist and get Raw URL

`ug` is a simple shell script tool to upload a file to GitHub Gist and return the raw URL.

## Background

Manually uploading files to GitHub Gist and then copying the raw URL is cumbersome and repetitive.  
This tool automates that process, allowing you to quickly upload a file and get the raw URL in one step, streamlining your workflow.

## Usage

```bash
ug <filename>
```

## Requirements & Setup

Before using `ug`, ensure you have the GitHub CLI installed and properly authenticated.

### Install GitHub CLI

On Debian/Ubuntu/macOS (with Homebrew), install with:

```bash
sudo apt install gh       # Debian/Ubuntu
# or
brew install gh           # macOS with Homebrew
```

### Authenticate with GitHub

Log in to GitHub via CLI (one-time setup):

```bash
gh auth login
```

Follow the prompts to authenticate, typically via a web browser.

### Check Authentication Status

To verify you are logged in:

```bash
gh auth status
```

## Example

Upload a file called `update.sh`:

```bash
ug update.sh
```

The script will output the raw URL of the uploaded gist.
