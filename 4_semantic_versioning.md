Divided by octets into 3. Versioning fallows:

2.1.0
[Major Version] - [Minor version] - [Patch version]

## Major version

Will not be backwords compatible with any previous major versions. Less frequent

## Minor version

More frequent. Has important features or changes.
Is compatible with all previous minor versions of that major version

## Patch updates:

bug fixes for this minor version

Example of a release cycle:

1.0.0 - first version
1.1.0 - new feature
1.1.1 - bug fix in new feature

1.2.0 - another new feature [resets patch version]

2.0.0 - major new version. After the project had to introduce breaking changes. Possible breaking changes to 1.0.0

## modifies

### ^

Most common is a carrot ^ - install latest minor version. This is used by yarn by deafult. It will never go above major 3. Also it will use this minor version as a lowest acceptable.

^3.2.1 - 3.2.1 -> 3.9.9

### ~

Does the same as ^ on the patch version
~3.2.1 - 3.2.1 -> 3.2.9

## exact/ =

if we have i.e 3.2.1 without modifier we will install this version and nothing else

## >, >=, <

Logical operators, greater, older etc

## \*

Install very latest version

## 3.\* / 3.x

most recent minor version

## range 3.1.5 - 3.2.2
