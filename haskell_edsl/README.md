# Checktestdata Haskell EDSL

This is a Haskell implementation of the checktestdata tool. The language is build as a Haskell EDSL with can be used to check a specific format of the data, as well as checking semantic correctness of the data. There is also an executable providing backwards compatibility with existing CTD scripts.

For building, a recent [Haskell compiler](https://www.haskell.org/ghc/) is needed, as well as a build tool such as [Cabal](https://www.haskell.org/cabal/) or [Stack](https://www.haskellstack.org/). For installing both the compiler and a build tool, [Haskell Platform](https://www.haskell.org/platform/) is recommended.

## Building with stack

For building with stack, run:
```
stack init
stack build
```

Then the executable can be run with:
```
stack exec checktestdata
```

The tests can be run with:
```
stack test
```

## Building with cabal

For building with cabal, run:
```
cabal install --only-dependencies
cabal configure
cabal build
```

Then the executable can be run with:
```
dist/build/checktestdata/checktestdata
```

The tests can be run with:
```
cabal test
```