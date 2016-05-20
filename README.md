Docker container for hacking on GHC on 32-bit platform
======================================================

This is a clone of
[gregweber/ghc-haskell-dev](https://hub.docker.com/r/gregweber/ghc-haskell-dev/)
that is based on [my 32-bit debian testing image
alexdzyoba/debian-testing-x86](https://hub.docker.com/r/alexdzyoba/debian-testing-x86/)

To start hacking, cd into ghc sources and say:

    $ sudo docker run --rm -i -t -v `pwd`:/home/ghc alexdzyoba/ghc-haskell-dev-x86 /usr/bin/linux32 /bin/bash

There you'll see that it's indeed 32-bit platform:

    ghc@e0bcb32c27b1:~$ arch
    i686
