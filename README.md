# [lduran2] / [git-unzip-all]

hooks a script to uncompress all files matching desired patterns after
to the pre-commit stage of a repo.

## How to download

Add this module to your repo from its root directory by using
```bash
git submodule add https://github.com/lduran2/git-unzip-all hooks/unzip-all
```

This command will download update `git-unzip-all` to
`hooks/unzip-all`, and update `.gitmodules` to associate the
submodule.

## How to install

### Requirements

#### In Windows

Installing requires use of the `git` command within a `bash` shell.
Allowing access to the `git` command, requires an extra step in
Windows operating systems. Namely, it requires adding `%git%/cmd` to
the `%PATH%` variable where `%git%` represents the directory of the Git
installation.  This depends on the location of Git and the operating
system, but may appear as follows

```batch
PATH=C:\git\cmd;%PATH%
```

where the assumed location of the Git installation is `C:\git\cmd`.

### Instructions

Then install it in the repo by using
```bash
bash hooks/unzip-all/git-config-pre-commit
```

This script adds the command to call the hook program `main` in the
root directory to this module to the  `pre-commit` hook for this repo,
thereby associating them through the call, then creates and stages a
template for the file of patterns to match files against for unzipping.

[lduran2]: https://github.com/lduran2
[git-unzip-all]: https://github.com/lduran2/git-unzip-all
