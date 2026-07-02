# Dotfiles backup

## Using stow utility to apply the dotfiles configuration
```bash
stow -t ~ folder_path
```

## How to insall stow
### APT package manager
```bash
sudo apt update
sudo apt install stow
```
### Download directly via http: [stow download link](https://ftp.gnu.org/gnu/stow/)

## How to use stow
- Symlink all files recursively to a given directory:
    `stow --target=path/to/target_directory file1 directory1 file2 directory2`

- Delete symlinks recursively from a given directory:
    `stow --delete --target=path/to/target_directory file1 directory1 file2 directory2`

- Simulate to see what the result would be like:
    `stow --simulate --target=path/to/target_directory file1 directory1 file2 directory2`

- Delete and resymlink:
    `stow --restow --target=path/to/target_directory file1 directory1 file2 directory2`

- Exclude files matching a regular expression:
    `stow --ignore=regular_expression --target=path/to/target_directory file1 directory1 file2 directory2`

