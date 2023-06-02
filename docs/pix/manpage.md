---
title: Manpage pix - KOOMPI OS
description: Manpage for the pix utility.
---

# Manpage `pix`

## NAME

```text
`pix` - the KOOMPI OS package manager that is easy to use with support for installing packages from multiple sources inside containers without altering the root filesystem.
```

## SYNOPSIS

```text
pix [options] [command] [arguments]
```

## DESCRIPTION

```markdown
pix is a wrapper around multiple package managers to install packages and run commands inside a managed container.

Usage:
    pix [options] [command] [arguments]

Options:
    -h, --help      Show this help message and exit
    -v, --version   Show version and exit
    --aur           Install packages from the AUR repository
    --dnf           Install packages from the Fedora repository

Commands:
    autoremove      Remove all unused packages
    clean           Clean the pix package manager cache
    enter           Enter the container shell
    export          Export/Recreate a program's desktop entry from the container
    help            Show this help message and exit
    init            Initialize a managed container
    install         Install packages inside the container
    list            List installed packages
    log             Show logs
    purge           Purge packages from the container
    run             Run a command inside the container
    remove          Remove packages from the container
    search          Search for packages
    show            Show details about a package
    unexport        Unexport/Remove a program's desktop entry
    update          Update the list of available packages
    upgrade         Upgrade the system by installing/upgrading available packages
```

## AUTOREMOVE

```markdown
Description: 
    Remove all unused packages automatically.
Usage:
    pix autoremove [options]

Options:
    -h, --help            Show this help message and exit

Usage:
    pix autoremove
```

## CLEAN

```markdown
Description: 
    Clean the pix package manager cache.

Usage:
    pix clean [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix clean
```

## ENTER

```markdown
Description: 
    Enter in the container shell.

Usage:
    pix enter [options]

Options:
    -h, --help            Show this help message and exit
```

## EXPORT

```markdown
Description: 
    Export/Recreate a program's desktop entry from a managed container.

Usage:
    pix export <program> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix export htop
```

## INIT

```markdown
Description: 
    Initialize the managed container.

Usage:
    pix init [options]

Options:
    -h, --help            Show this help message and exit
```

## INSTALL

```markdown
Description: 
    Install packages inside a managed container.

Usage:
    pix install [options] <packages>

Options:
    -h, --help            Show this help message and exit
    -y, --assume-yes      Proceed without manual confirmation.
    -f, --fix-broken      Fix broken deps before installing
    --no-export           Do not export a desktop entry after the installation. 
    --sideload [path]     Install a package from a local file.

Examples:
    pix install htop git
    pix install --sideload /path/to/file.deb
```

## LIST

```markdown
Description: 
    List installed packages.

Usage:
    pix list [options]

Options:
    -h, --help            Show this help message and exit
```

## PURGE

```markdown
Description: 
    Purge packages inside a managed container.

Usage:
    pix purge <packages> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix purge htop
```

## REMOVE

```markdown
Description:
    Remove packages inside a managed container.

Usage:
    pix remove <packages> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix remove htop
```

## RUN

```markdown
Description: 
    Run a program inside a managed container.

Usage:
    pix run <program> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix run htop
```

## SEARCH

```markdown
Description: 
    Search for packages in a managed container.

Usage:
    pix search <packages> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix search htop
```

## SHOW

```markdown
Description: 
    Show details about a package.

Usage:
    pix show <package> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix show htop
```

## UNEXPORT

```markdown
Description:
    Unexport/Remove a program's desktop entry from a managed container.

Usage:
    pix unexport <program> [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix unexport htop
```

## UPDATE

```markdown
Description: 
    Update the list of available packages.

Usage:
    pix update [options]

Options:
    -h, --help            Show this help message and exit

Examples:
    pix update
```

## UPGRADE

```markdown
Description: 
    Upgrade the system by installing/upgrading available packages.

Usage:
    pix upgrade [options]
  
Options:
    -h, --help            Show this help message and exit

Examples:
    pix upgrade
```

## VERSION

```markdown
Description:
    Display the version number of pix.

Usage:
    pix --version
    pix -v
```

## SEE ALSO

- [`abroot`](/docs/ABRoot)
- [`kso`](/docs/kso)

## AUTHOR

```text
Contributors of KOOMPI OS
```

## REPORTING BUGS

Report bugs to the [issue tracker](https://github.com/koompi-os/pix/issues).
