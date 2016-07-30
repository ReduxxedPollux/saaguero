## Mac
Get the latest macvim version with 
    
    brew install macvim --with-cscope --with-lua --HEAD

You can use `macvim -v` for terminal vim.

## Ubuntu
Compile from scratch following this [guide](http://zaiste.net/2013/05/compiling_vim_with_ruby_and_python_support_on_ubuntu/)

## Fedora
Ensure the following libraries are in place for having clipboard support:

```
sudo dnf install libX11-devel libSM-devel libXpm-devel libXt-devel libXtst-devel libXmu-devel
```

Then proceed with the regular compilation process, ie:

```
./configure \
 --with-features=huge \
 --enable-multibyte \
 --enable-pythoninterp \
 --with-x \
 --with-python-config-dir=/usr/lib/python2.7/config
make -j 4
sudo make install
```

## Windows
Use the latest compiled version from [here](http://solar-blogg.blogspot.ca/p/vim-build.html)

You can use terminal vim in Windows. I recommend doing it with the console emulator [cmder](http://bliker.github.io/cmder/)
