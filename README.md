Note: this branch adds a `nix/` directory, and `default.nix` and `shell.nix`
files to try building this package with Nix, and make it available as a
dependency for other projects (in particular `noteed/minicron` and
`noteed/humming`). In the future, those should use Thyme as provided by nixpkgs
(but it is marked as broken there, so this branch is also a step towards fixing
that too).


# thyme

[![CI](https://github.com/haskell-github-trust/thyme/actions/workflows/haskell.yml/badge.svg)](https://github.com/haskell-github-trust/thyme/actions/workflows/haskell.yml) [![Hackage](https://img.shields.io/hackage/v/thyme.svg?logo=haskell)](http://hackage.haskell.org/package/thyme)

A faster date and time library based on [time][].

* Trades speed for slightly less precision: micro- (μs; 10<sup>-6</sup>)
  versus pico-seconds (ps; 10<sup>-12</sup>).
* Better type-safety for date and time arithmetic.
* Ships with a selection of [Iso'][]s and [Lens'][]s for [lens][].

## Building

### Library

```
cabal build
```

### Haddock

```
cabal haddock
```

[Iso']: http://hackage.haskell.org/package/lens/docs/Control-Lens-Iso.html#t:Iso-39-
[Lens']: http://hackage.haskell.org/package/lens/docs/Control-Lens-Lens.html#t:Lens-39-
[lens]: http://hackage.haskell.org/package/lens
[time]: http://hackage.haskell.org/package/time

