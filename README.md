# wl-clipboard-history: Wayland clipboard history tracker

Simple bash script that uses [wl-clipboard](https://github.com/bugaevc/wl-clipboard) and sqlite to remember wayland clipboard history.

### Usage
    Usage: ./wl-clipboard-history OPTION [ARG]

       -t           Track clipboard changes
       -l [NUMBER]  Print last NUMBER of clipboard entries (defaults to 10 entries)
       -p [INDEX]   Print clipboard entry at INDEX (defaults to the last entry)

To use with [sway](https://github.com/swaywm/sway) add the following to your configuration:

    exec wl-clipboard-manager -t

There's also a [fzf](https://github.com/junegunn/fzf) wrapper for selecting the contents with a [TUI](https://github.com/janza/wl-clipboard-history/blob/master/contrib/fzf-wrapper).
