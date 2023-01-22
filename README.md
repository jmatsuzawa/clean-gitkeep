# clean-gitkeep
Remove unnecessary .gitkeep files.

This command runs `git rm` against unnecessary keep files (`.gitkeep` by default).
The tool decides a keep file is unnecessary, when the keep file is stored with other files on a directory.
If the tool finds only a keep file on a directory, it will not be removed.

## Install

Just copy `clean-gitkeep` script to one of the directories in your `PATH`.

## Usage

Basically just run `clean-gitkeep`, it recursively removes unnecessary `.gitkeep` files from the current directory:

```console
clean-gitkeep
```

### Specify directory containing keep files rather than current directory

Use `-d` option like:

```console
clean-gitkeep -d ./specific_directory
```

### Specify the name of keep files instead of `.gitkeep`

Use `-d` option like:

```console
clean-gitkeep -f .keep
```

It will remove every unnecessary `.keep`.
