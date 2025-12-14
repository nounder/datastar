# Datastar

Minimal fork of Star Federation's [data-star.dev](https://data-star.dev/) adjusted to be used in Bun & Deno:

1. `package.json` at the root of the repo so it can used directly by bun/npm.
2. no build step:
   - use relative imports instead of typescript aliases (works even with `node --strip-types`) ;
   - remove globals, like `ALIAS`.


## Usage

Add dependency:

```sh
bun add nounder/datastar
```

And in your project:

```
import "@nounder/datastar"
```

## Build

```sh
# update upstream repo
scripts/update

# copy and transform source code
scripts/build
```


