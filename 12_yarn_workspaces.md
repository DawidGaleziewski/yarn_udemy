monorepo method
packages like babel is using this method to keep all packages in one place.

Big advantage is the dependancies are shared as well as the code.

We need to specify in package.json array of workspaces

We can create a yarn init in each file.
After that we

Popular naming convention is to do something like:

@monorepo/server

where first part is the project name, second is the package

```js
  "workspaces": [
    "packages/*"
  ]
```
