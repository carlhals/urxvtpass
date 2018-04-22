# urxvtpassx
This extension integrates with 'pass' and 'zenity' to select and copy passwords to clipboar
It is useful when using the password manager in a virtualized environment, where copy-paste could be limited between hypervisor and VMs.
Otherwise the passmenu dmenu wrapper included with pass is recommended for easier access.

## Setup

1. Clone the repository and copy the **pass** script to wherever your URxvt extensions live (Sometimes __~/.urxvt/ext__)

2. Make sure the following exists somewhere in your .Xresources or .Xdefaults:
```
    URxvt.perl-ext-common:      pass
    URxvt.keysym.Mod-P:        perl:pass:copy
```
3. After merging the changes with `xrdb -merge ~/.Xresources` or something similar you can enjoy pass integration in a **new** urxvt-terminal by pressing _Super-Shift-p
