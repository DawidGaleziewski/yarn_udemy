similar like with --dev in npm
yarn provides us 5 dependency types.

Mostly we will be using just "dependencies" and "devDependencies"

## dependencies

Critical to project working

## devDependencies

Only for development

We can install those by:

```bash
yarn add --dev <package>
```

```json
{
  "name": "1_test_project",
  "version": "0.0.9",
  "main": "index.js",
  "license": "MIT",
  "dependencies": {
    "jquery": "^3.6.0"
  },
  "devDependencies": {
    "gulp": "^4.0.2"
  }
}
```

## peerDependencies

Applys when creating packages. Dependends on a package installed by the user, that can only exist ONCE.

I.E we want to create a plugin for grunt.

## optionalDependencies

We can use those but it not it wont break our code. I.E only for macs.

## bundled Dependencies

already installed in the packes that do not need to be downloaded and installed.

# installing dependencies

## yarn install

Will install all

## yarn install --production

will install only "dependencies" and ignore other types
