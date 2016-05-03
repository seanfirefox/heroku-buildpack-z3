# heroku-buildpack-z3

Fetches, compiles, and makes available the `z3` binary from
[Z3Prover/z3](https://github.com/Z3Prover/z3).

Exports `Z3_BINARY_PATH=/path/to/z3` as the path to the `z3` binary.

## Configure

Add to your projects buildpacks by running `heroku buildpacks:set
https://github.com/lawrencejones/heroku-buildpack-z3`. Make sure the ordering of
the buildpacks ensures that `z3` is run before any other installation steps that
may require access to the binary.
