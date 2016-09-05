# project structure

typical project structure looks like:

```
    ->project
        ->include
            ->includes.x
        ->src
            ->sources.x
        ->libraries (contains other sources that follow the same directory structure)
            ->projecty
        ->lib (contains src build into a librarie)
            ->libs.x
        Sconstruct
        README.md
        LICENSE.txt
```

# build modes

this build script enables three build modes namely:

```
$ scons devbuild
$ scons libbuild
$ scons
```
devbuild builds with development flags and debug flags.

such include -O0 and -ggdb3

libbuild builds like a release but instead builds a static library.

and the last without and build targets specified, builds a release version,

which turns on some optimizations.


