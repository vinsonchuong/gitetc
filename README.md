# gitetc
Scripts to help you track changes to your /etc files

After changing a file in `/etc` for the first time, track it using
`gitetc-add`. After subsequent changes or system updates, run `gitetc-sync` to
check for changes tracked files.

`gitetc` maintains a `git` repository located by default (see
[below](#configuration)) in `~/.gitetc/`.

## Scripts
* `gitetc-add` track a new `/etc` file
  ([docs](doc/gitetc-add.md), [code](bin/gitetc-add))
* `gitetc-rm` un-track an `/etc` file
  ([docs](doc/gitetc-rm.md), [code](bin/gitetc-rm))
* `gitetc-sync` checks `/etc` and updates all tracked files
  ([docs](doc/gitetc-sync.md), [code](bin/gitetc-sync))
* `gitetc-install` copies all tracked files to `/etc`
  ([docs](doc/gitetc-install.md), [code](bin/gitetc-install))

## Installing
If the target machine is running [Arch Linux](https://www.archlinux.org/),
an [AUR package](https://aur.archlinux.org/packages/gitetc/) is
available.

Otherwise, the scripts in the `bin` directory can be executed directly.

## Configuration
Change the location of the backing `git` repository via:
```sh
git config --global gitetc.path ~/projects/etcfiles
```
