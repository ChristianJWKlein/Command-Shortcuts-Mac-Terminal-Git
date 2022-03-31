# npm and yarn commands to master

commands to make you slick and quick

## 1. Packages Listing

Understand Libraries installed into your Machine Library.  
list/ls commands allow us to see installed dependencies and allow inspection of both local and global.

    yarn list [--depth] [--pattern]
    npm ls [[<@scope>/]<pkg> ...]
    npm list [[<@scope>/]<pkg> ...]

### Examples

#### list all directory deps

npm list

#### list all the global deps

npm list -g

#### list only first level of deps

npm list -g --depth 0

#### list the dependencies 4 levels deep

npm list -g --depth 4

#### yarn is slightly different

yarn list --pattern gulp

## 2. Package Presence

Why packages are installed. Direct dependency or co-dependency

#### using it with a package name

npm why react
yarn why react

#### using it with a package folder

npm why node_modules/loadsh

#### using it with a file inside a package

npm why node_modules/html-entities/lib/index.js

## 3. Package Info

Pull all info...dependencies, its maintainers, all its dist tags, ts latest release

#### prints regular console text info

npm info react

#### print info in JSON format

npm info react --json

## 4. Packages Licenses

##### will output all the packages and it's licenses urls

yarn licenses list

##### this will output of the licenses text

yarn licenses generate-disclaimer

#### ❌ not available in npm

## 5. Dependency Homepage

The below command will open a browser to the URL https://reactjs.org/ where we can find all the information we need about React.

    npm home react

    ❌ not available in yarn

## 6. Packages Outdated

    yarn outdated [package...]
    npm outdated [[<@scope>/]<pkg> ...]

#### checking the directory packages outdated

    npm outdated

### checking the global packages outdated

    npm outdated -g

#### it will skip the devDependencies

    npm outdated --prod

## 7. Packages Initialization

    npm init
    yarn init
    yarn

## 8. Upgrading Packages

We can upgrade dependencies by their name or use a pattern to accommodate a wider dependency list. We can also upgrade all dependencies of a given scope by using the --scope option.

    yarn upgrade [package]... --latest|-L [--caret | --tilde | --exact] [--pattern]
    npm update [-g] [<pkg>...]

#### using pattern

    yarn upgrade --pattern gulp

#### using pattern and dependency name

    yarn upgrade left-pad --pattern "gulp|grunt"

#### using the tag to indicate the dependency version we want

    yarn upgrade --latest --pattern "gulp-(match|newer)"

#### using scope

    yarn upgrade --scope @angular
