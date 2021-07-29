## Add the aliases

Add in `.bashrc`:

```
source /opt/infosec-tools/infosec-tools-bash-aliases
```

## Submodules

### Add a submodule

```
git submodule add gitrepourl
```

### Remove a submodule

```
# Remove the submodule entry from .git/config
git submodule deinit -f path/to/submodule

# Remove the submodule directory from the superproject's .git/modules directory
rm -rf .git/modules/path/to/submodule

# Remove the entry in .gitmodules and remove the submodule directory located at path/to/submodule
git rm -f path/to/submodule
```

### Update all submodules

```
git submodule update --recursive --remote
```
