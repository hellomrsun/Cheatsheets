# Npm cheat sheet

NPM: **Node Package Manager**

You need to install Node.js before use npm.

## Check node version

````bash
> node -v
````

![1](./Resources/node-v.PNG)

## Check npm version

````bash
> npm -v
````

![1](./Resources/npm-v.PNG)

## Initialize default package.json file

````bash
> npm init -y
````

![1](./Resources/npm-init.PNG)

## Install package locally on project

````bash
> Format: npm install package-name
> Ex: npm install lodash
````

![1](./Resources/npm-install-lodash.PNG)

lodash package is installed on:

> C:\Users\SUN\source\repos\Npm-command-cheatsheet\node_modules

## Uninstall local package

````bash
> Format: npm uninstall package-name
> Ex: npm uninstall lodash
````

![1](./Resources/npm-uninstall-lodash.PNG)

## Install global package

````bash
> Format: npm install package-name -g / --global
> Ex: npm install lodash -g
````

![1](./Resources/npm-install-lodash-global.PNG)

lodash package is installed on:

> C:\Users\SUN\AppData\Roaming\npm\node_modules\lodash

## Uninstall global package

````bash
> Format: npm uninstall package-name -g / --global
> Ex: npm uninstall lodash -g
````

![1](./Resources/npm-uninstall-lodash-global.PNG)

lodash package is removed from:

> C:\Users\SUN\AppData\Roaming\npm\node_modules\

## Install specific version of package

````bash
> Format: npm install package-name@version-number
> Ex: npm install lodash@4.17.4
````

![1](./Resources/npm-install-lodash-specific.PNG)

## Install latest version of package

````bash
> Format: npm install package-name@latest
> Ex: npm install lodash@latest
````

![1](./Resources/npm-install-lodash-latest.PNG)

## Install 3.5.*X* version range of package

````bash
> Format: npm install package-name@^version-number
> Ex: npm install lodash@^3.5.0
````

![1](./Resources/npm-install-lodash-latest-version-titled.PNG)

## Install version range of package and save in package.json

Save is default behavior when package.json file exists.

````bash
> Format: npm install package-name@version-number --save
> Ex: npm install lodash@4.17.4 --save
````

Package.json:

![1](./Resources/npm-install-lodash-specific-dependencies.PNG)

## Install version  of package and save the exact version in package.json

````bash
> Format: npm install package-name@version-number --save-exact
> Ex: npm install lodash@4.17.4 --save-exact
````

Package.json:

![1](./Resources/npm-install-lodash-specific-dependencies-save-exact.PNG)


Set prxoy:

````bash
> npm config set proxy http://{domain}%5C{account}:{password}@{proxy}:{port}
````

Check proxy:

````bash
> npm get proxy
````

You can also check file : C:\Users\\{user_profile}\\.npmrc
