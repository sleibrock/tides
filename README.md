Tides
======


A collection of notes/programs using [TidalCycles](https://tidalcycles.org/index.php/Welcome).


## Installation of TidalCycles

[Follow the notes for installation on TidalCycles' wiki page](). Once you have [Haskell]() and [SuperCollider]() installed, you will have to configure your audio for it properly (on Linux, you will need to use JACK).

Then, to install TidalCycles, you need to install it from `cabal`. But you must first configure `~/.cabal/config` in order to get GHC to link and build properly.

Open up `~/.cabal/config` and configure the options below with the following values:
```
library-vanilla: False
shared: True
executable-dynamic: True
ghc-options:
  -dynamic
```

Then you should be ready to start running TidalCycles. Set up your audio routing (run JACK first), then turn on SuperCollider, then initialize the TidalCycles server, then you can run an editor to edit code with TidalCycles.
