# gitetc-add(1) -- track a new /etc file

## SYNOPSIS
`gitetc-add` `-h`|`--help`<br>
`gitetc-add` _file_ ...<br>

## DESCRIPTION
`gitetc-add` tracks a new `/etc` file by adding it to the backing repository.
By default, the repository is in `~/.gitetc`. Its location can be configured
using `git config --global gitetc.path _path_`. A repository will be created
if it doesn't already exist.

## OPTIONS
* -h, --help:
  Show help text and exit.

## COPYRIGHT
`gitetc` is Copyright (c) 2015 Vinson Chuong under the MIT License.
