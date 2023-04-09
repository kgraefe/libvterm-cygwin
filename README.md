# libvterm-cygwin

This a recipe to build and package [libvterm][1] for [Cygwin][2]. The recipe
is based on the [recipe in cascent's old neovim port][3].

To build run the following command:
```sh
cygport libvterm.cygport download prepare compile install package
```

To install the package you can extract it into the root directory:
```sh
eval "$(cygport libvterm.cygport vars PVR)"
tar -C / -xjvf libvterm-$PVR.x86_64/dist/libvterm/libvterm/libvterm0/libvterm-$PVR.tar.xz
```

[1]: http://www.leonerd.org.uk/code/libvterm/
[2]: http://www.cygwin.com/
[3]: https://github.com/cascent/neovim-cygwin/blob/09277e3f76981189a2f15d1dbc2f5a4ab4b6c86f/libvterm/libvterm.cygport
