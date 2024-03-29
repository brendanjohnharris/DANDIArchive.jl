# DANDIArchive
[![](https://img.shields.io/badge/docs-dev-blue.svg)](https://brendanjohnharris.github.io/DANDIArchive.jl/dev)
[![Build Status](https://github.com/brendanjohnharris/DANDIArchive.jl/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/brendanjohnharris/DANDIArchive.jl/actions/workflows/CI.yml?query=branch%3Amain)
[![Coverage](https://codecov.io/gh/brendanjohnharris/DANDIArchive.jl/branch/main/graph/badge.svg)](https://codecov.io/gh/brendanjohnharris/DANDIArchive.jl)

This little package wraps functions from the [Dandi](https://dandiarchive.org/) [python](https://github.com/dandi/dandi-cli) API.

Functions and classes from the python API can be accessed with:
```julia
using DANDIArchive
DANDIArchive.<module>.<function>
```
where valid values for `<module>` and `<function>` generally follow the documentation for the python package, available [here](https://dandi.readthedocs.io/en/latest/).

Additional functions have been added for convenience, such as:
```julia
dandiurl(dandiset_id::String, filepath::String; version::{String})
```
which can be used to grab the url of a dandiset from the dandiset id and the filepath of the file within the dandiset.