# yarn link

Live package testing

we can link the package. This will allow us to install local packages as if they were pulled from registry

yarn link # in the package.json dir of our package
yarn link nasme_of_the_package # in the dir we want to instrall the package in

What is more it will be linked to those files directly.
This will auto change files in node_modules

we can remove link by:
yarn unlink

# yarn pack

create a archive same way it would be published to the registry. In tgz format

we can then add the package by

yarn add ~/dir_to_archive/package.tgz

# publish pack to npm registry

yarnpkg.com api will use npm and is the preffered registry at this time.

we also should (but dont have to) publish the package to github. As it will allow users to submit issues and work on the package.

We also should add things like kewyeords in package.json

run yarn publish once ready

# update version

run: to change version
yarn version
yarn publish

now it can be updated by yarn upgrade
