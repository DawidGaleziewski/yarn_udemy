# yarn list

show dependency graph

# yarn why <dependency>

Usefull command that tells us the reasons this package was installed

=> Found "loose-envify@1.4.0"
info Reasons this module exists

- "react" depends on it
- Hoisted from "react#loose-envify"
  info Disk size without dependencies: "32KB"
  info Disk size with unique dependencies: "60KB"
  info Disk size with transitive dependencies: "60KB"
  info Number of shared dependencies: 1
  Done in 0.13s.

## package hoisiting

When package is shared dep by express and another package, yarn will hoist it, so that it does not have to install it one more time.

## yarn info

Will query package registry for information
yarn info underscore
