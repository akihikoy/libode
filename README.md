OVERVIEW
================
This is an archive of Open Dynamics Engine.

http://www.ode.org/

The files are obtained from the above website.

LICENSE
================
Refer to the license of ODE:

http://www.ode.org/ode-license.html

INSTALLATION
================
Quick note of installation on Linux (Ubuntu).

You may need autotools (Linux)

If you haven't installed OpenGL library,

    sudo apt-get -f install libglut3 libglut3-dev

Install ODE:

    $ mkdir ~/prg
    $ cd ~/prg
    $ git clone https://github.com/akihikoy/libode.git
    $ cd libode
    $ tar jxvf arc/ode-0.13.tar.bz2
    $ cd ode-0.13
    (Older versions:                               )
    (   $ ./configure --with-double-precision      )
    Newer versions:
        $ ./configure --enable-double-precision --enable-shared
    (Build with a single CPU:  )
    (   $ make                 )
    If you have many cores:
        $ make -j8

Other configure options:

    --disable-asserts    Disabling assertions in execution.

TEST
================
Run demos in ode/demo/

Fun demos I like:

    ode/demo/demo_chain1
    ode/demo/demo_chain2
    ode/demo/demo_buggy
    ode/demo/demo_crash
    ode/demo/demo_boxstack
