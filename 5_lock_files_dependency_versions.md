## yarn.lock

this file role is to ensure the version and the dependency tree will be the same when cloned

yarn.lock should be alway commited with the project and NEVER edited directly

Some information in the yarn.lock regarding the dependencies:

```yarn
underscore@^1.13.1: # Underscore specified at version range
  version "1.13.1" # version installed (aka resolved)
  resolved "https://registry.yarnpkg.com/underscore/-/underscore-1.13.1. # where the version was installed from
  tgz#0c1c6bd2df54b6b69f2314066d65b6cde6fcf9d1"
  integrity sha512-hzSoAVtJF+3ZtiFX0VgfFPHEDRm7Y/QPjGyNo4TVdnDTdft3tr8hEkD25a1jC+TjTuE7tkHGKkhwCgs9dgBB2g==
```

When we want to modify the version we want to:

1. update it in package.json
2. run yarn install

This will modify the yarn.lock automaticaslly

```yarn
underscore@1.3.1:
  version "1.3.1"
  resolved "https://registry.yarnpkg.com/underscore/-/underscore-1.3.1.tgz#6cb8aad0e77eb5dbbfb54b22bcd8697309cf9641"
  integrity sha1-bLiq0Od+tdu/tUsivNhpcwnPlkE=
```

or simply install the package once again with the specified version/version range:

```bash
yarn install underscore@1.*
yarn install underscore@^1.3.1
```

## yarn upgrade

yarn.lock will keep the same version that we had installed on original machine:
version "1.3.1"

therefore even if the version in package.json is ^1.3.1, and we have 1.8.1 available, it wont automatically bump it. We have to run.

It is important to remember that yarn upgrade will respect the version in the package.json

```bash
yarn upgrade underscore
```

This will bump our version to 1.8.1 (allowed one).

## yarn outdated

Will inform us when dependencies are allowed the be upgraded pass their allowed range. What is the newest version etc.
