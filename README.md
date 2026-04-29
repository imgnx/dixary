# `imgnx/dixary`

Words. Here.

## Installation

### Step 1: Copy

> 1. Make a copy of your .dic file (this one strips it of [`hunspell`](https://github.com/hunspell/hunspell)'s semantic marks):

```shellscript
# ie. Copy a stripped version of the .dic file to your clipboard
sed '1d; s#/.*##' en_US.dic | sort -u | pbcopy

# ie. Paste that into a file in a local, shared directory
pbpaste > ~/.local/share/hunspell/en_US.dic
```

### Step 2: Paste

> Add this to your `~/.bashrc` (most Linux) or `~/.zshrc` (macOS):

#### ie. English, USA

```shellscript
export WORDS="~/.local/share/hunspell/en_US.dic"
```

#### ie. Latin

```

export WORDS="~/.local/share/hunspell/la.dic"

```
