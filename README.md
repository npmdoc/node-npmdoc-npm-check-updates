# api documentation for  [npm-check-updates (v2.10.4)](https://github.com/tjunnone/npm-check-updates)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-npm-check-updates.svg)](https://travis-ci.org/npmdoc/node-npmdoc-npm-check-updates)
#### Find newer versions of dependencies than what your package.json or bower.json allows

[![NPM](https://nodei.co/npm/npm-check-updates.png?downloads=true)](https://www.npmjs.com/package/npm-check-updates)

[![apidoc](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-npm-check-updates_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-npm-check-updates/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Tomas Junnonen",
        "email": "tomas1@gmail.com"
    },
    "bin": {
        "npm-check-updates": "./bin/npm-check-updates",
        "ncu": "./bin/ncu"
    },
    "bugs": {
        "url": "https://github.com/tjunnone/npm-check-updates/issues"
    },
    "contributors": [
        {
            "name": "Raine Revere",
            "url": "https://github.com/raineorshine"
        }
    ],
    "dependencies": {
        "bluebird": "^3.4.3",
        "chalk": "^1.1.3",
        "cint": "^8.2.1",
        "cli-table": "^0.3.1",
        "commander": "^2.9.0",
        "fast-diff": "^1.0.1",
        "find-up": "1.1.2",
        "get-stdin": "^5.0.1",
        "json-parse-helpfulerror": "^1.0.3",
        "lodash": "^4.15.0",
        "node-alias": "^1.0.4",
        "npm": "^3.10.6",
        "npmi": "^2.0.1",
        "require-dir": "^0.3.0",
        "semver": "^5.3.0",
        "semver-utils": "^1.1.1",
        "snyk": "^1.25.1",
        "spawn-please": "^0.2.0",
        "update-notifier": "^1.0.2"
    },
    "description": "Find newer versions of dependencies than what your package.json or bower.json allows",
    "devDependencies": {
        "chai": "^3.5.0",
        "chai-as-promised": "^6.0.0",
        "chai-string": "^1.2.0",
        "chokidar-cli": "^1.2.0",
        "eslint": "^3.4.0",
        "mocha": "^3.0.2",
        "should": "^11.1.0",
        "tmp": "0.0.31"
    },
    "directories": {},
    "dist": {
        "shasum": "0833dd707f983a04fdcd615afb860ce82b1e54a2",
        "tarball": "https://registry.npmjs.org/npm-check-updates/-/npm-check-updates-2.10.4.tgz"
    },
    "dynamicDependencies": {
        "bower": "^1.6.5"
    },
    "engines": {
        "node": ">=0.12"
    },
    "files": [
        "bin",
        "lib"
    ],
    "gitHead": "14dfe6928fea79a9630f86d1b1039e5a8832fbcc",
    "homepage": "https://github.com/tjunnone/npm-check-updates",
    "keywords": [
        "npm",
        "bower",
        "check",
        "find",
        "discover",
        "updates",
        "upgrades",
        "dependencies",
        "package.json",
        "bower.json",
        "updater",
        "version",
        "management"
    ],
    "license": "Apache-2.0",
    "main": "./lib/npm-check-updates",
    "maintainers": [
        {
            "name": "tjunnone",
            "email": "tomas1@gmail.com"
        },
        {
            "name": "raine",
            "email": "raineorshine@gmail.com"
        }
    ],
    "name": "npm-check-updates",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tjunnone/npm-check-updates.git"
    },
    "scripts": {
        "lint": "eslint bin lib test",
        "test": "npm run lint ; mocha && mocha test/individual",
        "watch": "chokidar \"lib/**/*.js\" -c \"npm run test\""
    },
    "version": "2.10.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module npm-check-updates](#apidoc.module.npm-check-updates)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>getCurrentDependencies (pkgData, options)](#apidoc.element.npm-check-updates.getCurrentDependencies)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>getGreatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.getGreatestPackageVersion)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>getInstalledPackages (options)](#apidoc.element.npm-check-updates.getInstalledPackages)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>getLatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.getLatestPackageVersion)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>getPreferredWildcard (dependencies)](#apidoc.element.npm-check-updates.getPreferredWildcard)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>getVersionTarget (options)](#apidoc.element.npm-check-updates.getVersionTarget)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>initialize (args)](#apidoc.element.npm-check-updates.initialize)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>isSatisfied (version, range, loose)](#apidoc.element.npm-check-updates.isSatisfied)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>isUpgradeable (current, latest)](#apidoc.element.npm-check-updates.isUpgradeable)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>queryVersions (packageMap, options)](#apidoc.element.npm-check-updates.queryVersions)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>run (opts)](#apidoc.element.npm-check-updates.run)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradeDependencies (currentDependencies, latestVersions, options)](#apidoc.element.npm-check-updates.upgradeDependencies)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradeDependencyDeclaration (declaration, latestVersion, options)](#apidoc.element.npm-check-updates.upgradeDependencyDeclaration)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradePackageData (pkgData, oldDependencies, newDependencies, newVersions, options)](#apidoc.element.npm-check-updates.upgradePackageData)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradePackageDefinitions (currentDependencies, options)](#apidoc.element.npm-check-updates.upgradePackageDefinitions)
1.  object <span class="apidocSignatureSpan">npm-check-updates.</span>version_util
1.  object <span class="apidocSignatureSpan">npm-check-updates.</span>versionmanager

#### [module npm-check-updates.version_util](#apidoc.module.npm-check-updates.version_util)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>addWildCard (version, wildcard)](#apidoc.element.npm-check-updates.version_util.addWildCard)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>colorizeDiff (strToColor, strToCompare, options)](#apidoc.element.npm-check-updates.version_util.colorizeDiff)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>findGreatestByLevel (versions, current, level)](#apidoc.element.npm-check-updates.version_util.findGreatestByLevel)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>getPrecision (version)](#apidoc.element.npm-check-updates.version_util.getPrecision)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>isWildCard (version)](#apidoc.element.npm-check-updates.version_util.isWildCard)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>isWildPart (versionPart)](#apidoc.element.npm-check-updates.version_util.isWildPart)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>numParts (version)](#apidoc.element.npm-check-updates.version_util.numParts)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>precisionAdd (precision, n)](#apidoc.element.npm-check-updates.version_util.precisionAdd)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>setPrecision (version, precision)](#apidoc.element.npm-check-updates.version_util.setPrecision)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>stringify (semver, precision)](#apidoc.element.npm-check-updates.version_util.stringify)
1.  object <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>VERSION_ADDED_PARTS
1.  object <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>VERSION_BASE_PARTS
1.  object <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>VERSION_PARTS
1.  object <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>WILDCARDS

#### [module npm-check-updates.versionmanager](#apidoc.module.npm-check-updates.versionmanager)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getCurrentDependencies (pkgData, options)](#apidoc.element.npm-check-updates.versionmanager.getCurrentDependencies)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getGreatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.versionmanager.getGreatestPackageVersion)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getInstalledPackages (options)](#apidoc.element.npm-check-updates.versionmanager.getInstalledPackages)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getLatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.versionmanager.getLatestPackageVersion)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getPreferredWildcard (dependencies)](#apidoc.element.npm-check-updates.versionmanager.getPreferredWildcard)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getVersionTarget (options)](#apidoc.element.npm-check-updates.versionmanager.getVersionTarget)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>initialize (args)](#apidoc.element.npm-check-updates.versionmanager.initialize)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>isSatisfied (version, range, loose)](#apidoc.element.npm-check-updates.versionmanager.isSatisfied)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>isUpgradeable (current, latest)](#apidoc.element.npm-check-updates.versionmanager.isUpgradeable)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>queryVersions (packageMap, options)](#apidoc.element.npm-check-updates.versionmanager.queryVersions)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradeDependencies (currentDependencies, latestVersions, options)](#apidoc.element.npm-check-updates.versionmanager.upgradeDependencies)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradeDependencyDeclaration (declaration, latestVersion, options)](#apidoc.element.npm-check-updates.versionmanager.upgradeDependencyDeclaration)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradePackageData (pkgData, oldDependencies, newDependencies, newVersions, options)](#apidoc.element.npm-check-updates.versionmanager.upgradePackageData)
1.  [function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradePackageDefinitions (currentDependencies, options)](#apidoc.element.npm-check-updates.versionmanager.upgradePackageDefinitions)



# <a name="apidoc.module.npm-check-updates"></a>[module npm-check-updates](#apidoc.module.npm-check-updates)

#### <a name="apidoc.element.npm-check-updates.getCurrentDependencies"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>getCurrentDependencies (pkgData, options)](#apidoc.element.npm-check-updates.getCurrentDependencies)
- description and source-code
```javascript
function getCurrentDependencies(pkgData, options) {

    pkgData = pkgData || {};
    options = options || {};

    if (!options.prod && !options.dev && !options.optional) {
        options.prod = options.dev = options.optional = true;
    }

    var allDependencies = cint.filterObject(_.merge({},
        options.prod && pkgData.dependencies,
        options.dev && pkgData.devDependencies,
        options.optional && pkgData.optionalDependencies
    ), filterAndReject(options.filter, options.reject));

    return allDependencies;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.getGreatestPackageVersion"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>getGreatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.getGreatestPackageVersion)
- description and source-code
```javascript
getGreatestPackageVersion = function (pkgData) {
    return selectedPackageManager.greatest(pkgData);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.getInstalledPackages"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>getInstalledPackages (options)](#apidoc.element.npm-check-updates.getInstalledPackages)
- description and source-code
```javascript
function getInstalledPackages(options) {

    options = options || {};

    return selectedPackageManager.list([], {cwd: options.cwd}).then(function (results) {
        if (!results || !results.dependencies) {
            throw new Error('Unable to retrieve NPM package list');
        }

        // filter out undefined packages or those with a wildcard
        var filterFunction = filterAndReject(options.filter, options.reject);
        var validPackages = cint.filterObject(results.dependencies, function (dep, pkgInfo) {
            return pkgInfo && pkgInfo.name && pkgInfo.version && !versionUtil.isWildPart(pkgInfo.version) && filterFunction(dep);
        });

        // convert the dependency object from npm into a simple object that maps the package name to its version
        var simpleDependencies = cint.mapObject(validPackages, function (dep, pkgInfo) {
            return cint.keyValue(dep, pkgInfo.version);
        });

        return simpleDependencies;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.getLatestPackageVersion"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>getLatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.getLatestPackageVersion)
- description and source-code
```javascript
getLatestPackageVersion = function (pkgData) {
    return selectedPackageManager.latest(pkgData);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.getPreferredWildcard"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>getPreferredWildcard (dependencies)](#apidoc.element.npm-check-updates.getPreferredWildcard)
- description and source-code
```javascript
function getPreferredWildcard(dependencies) {

    // if there are no dependencies, return null.
    if (Object.keys(dependencies).length === 0) {
        return null;
    }

    // group the dependencies by wildcard
    var groups = _.groupBy(_.values(dependencies), function (dep) {
        return _.find(versionUtil.WILDCARDS, function (wildcard) {
            return dep && dep.indexOf(wildcard) > -1;
        });
    });

    // if none of the dependencies use a wildcard, return null
    var usedWildcards = Object.keys(groups);
    if (usedWildcards.length === 1 && usedWildcards[0] === 'undefined') {
        return null;
    }

    // convert to an array of objects that can be sorted
    var arrOfGroups = cint.toArray(groups, function (wildcard, instances) {
        return {
            wildcard: wildcard,
            instances: instances
        };
    });

    // reverse sort the groups so that the wildcard with the most appearances is at the head, then return it.
    var sorted = _.sortBy(arrOfGroups, function (wildcardObject) {
        return -wildcardObject.instances.length;
    });

    return sorted[0].wildcard;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.getVersionTarget"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>getVersionTarget (options)](#apidoc.element.npm-check-updates.getVersionTarget)
- description and source-code
```javascript
function getVersionTarget(options) {
    return options.semverLevel ? options.semverLevel :
        options.newest ? 'newest' :
        options.greatest ? 'greatest' :
        'latest';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.initialize"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>initialize (args)](#apidoc.element.npm-check-updates.initialize)
- description and source-code
```javascript
function initialize(args) {

    args = args || {};
    args.packageManager = args.packageManager || 'npm';

    if (!(args.packageManager in packageManagers)) {
        throw new Error('Invalid package manager: ' + args.packageManager);
    }

    selectedPackageManager = packageManagers[args.packageManager];

    return selectedPackageManager.init({
        global: args.global,
        registry: args.registry
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.isSatisfied"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>isSatisfied (version, range, loose)](#apidoc.element.npm-check-updates.isSatisfied)
- description and source-code
```javascript
function satisfies(version, range, loose) {
  try {
    range = new Range(range, loose);
  } catch (er) {
    return false;
  }
  return range.test(version);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.isUpgradeable"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>isUpgradeable (current, latest)](#apidoc.element.npm-check-updates.isUpgradeable)
- description and source-code
```javascript
function isUpgradeable(current, latest) {

    // do not upgrade non-npm version declarations (such as git tags)
    // do not upgrade versionUtil.wildcards
    if (!semver.validRange(current) || versionUtil.isWildCard(current)) {
        return false;
    }

    // remove the constraint (e.g. ^1.0.1 -> 1.0.1) to allow upgrades that satisfy the range, but are out of date
    var range = semverutils.parseRange(current)[0];
    if (!range) {
        throw new Error('"' + current + '" could not be parsed by semver-utils. This is probably a bug. Please file an issue at
https://github.com/tjunnone/npm-check-updates.');
    }
    var version = versionUtil.stringify(range);

    // make sure it is a valid range
    // not upgradeable if the latest version satisfies the current range
    // not upgradeable if the specified version is newer than the latest (indicating a prerelease version)
    return Boolean(semver.validRange(version)) &&
        !isSatisfied(latest, version) &&
        !semver.ltr(latest, version);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.queryVersions"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>queryVersions (packageMap, options)](#apidoc.element.npm-check-updates.queryVersions)
- description and source-code
```javascript
function queryVersions(packageMap, options) {

    var getPackageVersion;
    options = options || {};

    var packageList = Object.keys(packageMap);

    // validate options.versionTarget
    options.versionTarget = options.versionTarget || 'latest';

    // determine the getPackageVersion function from options.versionTarget
    switch (options.versionTarget) {
        case 'latest':
            getPackageVersion = selectedPackageManager.latest;
            break;
        case 'greatest':
            getPackageVersion = selectedPackageManager.greatest;
            break;
        case 'newest':
            getPackageVersion = selectedPackageManager.newest;
            break;
        case 'major':
            getPackageVersion = selectedPackageManager.greatestMajor;
            break;
        case 'minor':
            getPackageVersion = selectedPackageManager.greatestMinor;
            break;
        default:
            var supportedVersionTargets = ['latest', 'newest', 'greatest', 'major', 'minor'];
            return Promise.reject(new Error('Unsupported versionTarget: ' + options.versionTarget +
                '. Supported version targets are: ' + supportedVersionTargets.join(', ')));
    }

    // ignore 404 errors from getPackageVersion by having them return null instead of rejecting
    function getPackageVersionProtected(dep) {
        return getPackageVersion(dep, packageMap[dep]).catch(function (err) {
            if (err.message == 404) { // eslint-disable-line eqeqeq
                return null;
            } else {
                throw err;
            }
        });
    }

    // zip up the array of versions into to a nicer object keyed by package name
    function zipVersions(versionList) {
        return cint.toObject(versionList, function (version, i) {
            return cint.keyValue(packageList[i], version);
        });
    }

    return Promise.map(packageList, getPackageVersionProtected)
        .then(zipVersions)
        .then(_.partialRight(_.pickBy, _.identity));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.run"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>run (opts)](#apidoc.element.npm-check-updates.run)
- description and source-code
```javascript
function run(opts) {
    options = opts || {};

    // if not executed on the command-line (i.e. executed as a node module), set some defaults
    if (!options.cli) {
        _.defaults(options, {
            // if they want to modify the package file, we must disable jsonUpgraded
            // otherwise the write operation will not happen
            jsonUpgraded: !options.upgrade,
            // should not suggest upgrades to versions within the specified version range if upgradeAll is explicitly set to false
. Will become the default in the next major version.
            upgradeAll: options.upgradeAll === undefined ? true : options.upgradeAll,
            loglevel: 'silent',
            args: []
        });
    }

    // get filter from arguments
    options.filter = options.args.join(' ') || options.filter;

    print('Initializing...', 'verbose');

    return vm.initialize({
        global: options.global,
        packageManager: options.packageManager,
        registry: options.registry
    })
    .then(function () {

        options = initOptions(options);

        return options.global ?
            analyzeGlobalPackages() :
            findPackage().spread(analyzeProjectDependencies);
    });
}
```
- example usage
```shell
...
Integration
--------------
The tool allows integration with 3rd party code:

'''js
const ncu = require('npm-check-updates');

ncu.run({
    // Always specify the path to the package file
    packageFile: 'package.json',
    // Any command-line option can be specified here.
    // These are set by default:
    silent: true,
    jsonUpgraded: true
}).then((upgraded) => {
...
```

#### <a name="apidoc.element.npm-check-updates.upgradeDependencies"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradeDependencies (currentDependencies, latestVersions, options)](#apidoc.element.npm-check-updates.upgradeDependencies)
- description and source-code
```javascript
function upgradeDependencies(currentDependencies, latestVersions, options) {

    options = options || {};

    // filter out dependencies with empty values
    currentDependencies = cint.filterObject(currentDependencies, function (key, value) {
        return value;
    });

    // get the preferred wildcard and bind it to upgradeDependencyDeclaration
    var wildcard = getPreferredWildcard(currentDependencies) || DEFAULT_WILDCARD;
    var upgradeDep = _.partialRight(upgradeDependencyDeclaration, {
        wildcard: wildcard,
        removeRange: options.removeRange
    });

    return _(currentDependencies)
        // only include packages for which a latest version was fetched
        .pickBy(function (current, packageName) {
            return packageName in latestVersions;
        })
        // combine the current and latest dependency objects into a single object keyed by packageName and containing
        // both versions in an array: [current, latest]
        .mapValues(function (current, packageName) {
            var latest = latestVersions[packageName];
            return [current, latest];
        })
        // pick the packages that are upgradeable
        // we can use spread because isUpgradeable and upgradeDependencyDeclaration both take current and latest as
        // arguments
        .pickBy(_.spread(isUpgradeable))
        .mapValues(_.spread(upgradeDep))
        .value();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.upgradeDependencyDeclaration"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradeDependencyDeclaration (declaration, latestVersion, options)](#apidoc.element.npm-check-updates.upgradeDependencyDeclaration)
- description and source-code
```javascript
function upgradeDependencyDeclaration(declaration, latestVersion, options) {

    options = options || {};
    options.wildcard = options.wildcard || DEFAULT_WILDCARD;

    // parse the latestVersion
    // return original declaration if latestSemver is invalid
    var latestSemver = semverutils.parseRange(latestVersion)[0];
    if (!latestSemver) {
        return declaration;
    }

    // return global versionUtil.wildcards immediately
    if (options.removeRange) {
        return latestVersion;
    } else if (versionUtil.isWildCard(declaration)) {
        return declaration;
    }

    // parse the declaration
    // if multiple ranges, use the semver with the least number of parts
    var parsedRange = _(semverutils.parseRange(declaration))
        // semver-utils includes empty entries for the || and - operators. We can remove them completely
        .reject({operator: '||'})
        .reject({operator: '-'})
        .sortBy(_.ary(_.flow(versionUtil.stringify, versionUtil.numParts), 1))
        .value();
    var declaredSemver = parsedRange[0];

<span class="apidocCodeCommentSpan">    /**
     * Chooses version parts between the declared version and the latest.
     * Base parts (major, minor, patch) are only included if they are in the original declaration.
     * Added parts (release, build) are always included. They are only present if we are checking --greatest versions
     * anyway.
    */
</span>    function chooseVersion(part) {
        return versionUtil.isWildPart(declaredSemver[part]) ? declaredSemver[part] :
            _.includes(versionUtil.VERSION_BASE_PARTS, part) && declaredSemver[part] ? latestSemver[part] :
            _.includes(versionUtil.VERSION_ADDED_PARTS, part) ? latestSemver[part] :
            undefined;
    }

    // create a new semver object with major, minor, patch, build, and release parts
    var newSemver = cint.toObject(versionUtil.VERSION_PARTS, function (part) {
        return cint.keyValue(part, chooseVersion(part));
    });
    var newSemverString = versionUtil.stringify(newSemver);
    var version = v(declaredSemver.semver) + newSemverString;

    // determine the operator
    // do not compact, because [undefined, '<'] must be differentiated from ['<']
    var uniqueOperators = _(parsedRange)
        .map(function (range) {
            return range.operator;
        })
        .uniq()
        .value();
    var operator = uniqueOperators[0] || '';

    var hasWildCard = versionUtil.WILDCARDS.some(_.partial(_.includes, newSemverString, _, 0));
    var isLessThan = uniqueOperators[0] === '<' || uniqueOperators[0] === '<=';
    var isMixed = uniqueOperators.length > 1;

    // convert versions with </<= or mixed operators into the preferred wildcard
    // only do so if the new version does not already contain a wildcard
    return !hasWildCard && (isLessThan || isMixed) ?
        versionUtil.addWildCard(version, options.wildcard) :
        operator + version;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.upgradePackageData"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradePackageData (pkgData, oldDependencies, newDependencies, newVersions, options)](#apidoc.element.npm-check-updates.upgradePackageData)
- description and source-code
```javascript
function upgradePackageData(pkgData, oldDependencies, newDependencies, newVersions, options) {

    options = options || {};

    for (var dependency in newDependencies) {
        if (options.upgradeAll || !isSatisfied(newVersions[dependency], oldDependencies[dependency])) {
            var expression = '"' + dependency + '"\\s*:\\s*"' + escapeRegexp(oldDependencies[dependency] + '"');
            var regExp = new RegExp(expression, 'g');
            pkgData = pkgData.replace(regExp, '"' + dependency + '": ' + '"' + newDependencies[dependency] + '"');
        }
    }

    return pkgData;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.upgradePackageDefinitions"></a>[function <span class="apidocSignatureSpan">npm-check-updates.</span>upgradePackageDefinitions (currentDependencies, options)](#apidoc.element.npm-check-updates.upgradePackageDefinitions)
- description and source-code
```javascript
function upgradePackageDefinitions(currentDependencies, options) {
    var versionTarget = getVersionTarget(options);

    return queryVersions(currentDependencies, {
        versionTarget: versionTarget,
        registry: options.registry ? options.registry : null
    }).then(function (latestVersions) {

        var upgradedDependencies = upgradeDependencies(currentDependencies, latestVersions, {
            removeRange: options.removeRange
        });

        var filteredUpgradedDependencies = _.pickBy(upgradedDependencies, function (v, dep) {
            return !options.jsonUpgraded || options.upgradeAll || !isSatisfied(latestVersions[dep], currentDependencies[dep]);
        });

        return [filteredUpgradedDependencies, latestVersions];
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.npm-check-updates.version_util"></a>[module npm-check-updates.version_util](#apidoc.module.npm-check-updates.version_util)

#### <a name="apidoc.element.npm-check-updates.version_util.addWildCard"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>addWildCard (version, wildcard)](#apidoc.element.npm-check-updates.version_util.addWildCard)
- description and source-code
```javascript
function addWildCard(version, wildcard) {
    return wildcard === '^' || wildcard === '~' ?
        wildcard + version :
        setPrecision(version, 'major') + wildcard;
}
```
- example usage
```shell
...
   var hasWildCard = versionUtil.WILDCARDS.some(_.partial(_.includes, newSemverString, _, 0));
   var isLessThan = uniqueOperators[0] === '<' || uniqueOperators[0] === '<=';
   var isMixed = uniqueOperators.length > 1;

   // convert versions with </<= or mixed operators into the preferred wildcard
   // only do so if the new version does not already contain a wildcard
   return !hasWildCard && (isLessThan || isMixed) ?
       versionUtil.addWildCard(version, options.wildcard) :
       operator + version;
}

/**
* Upgrade a dependencies collection based on latest available versions
* @param currentDependencies current dependencies collection object
* @param latestVersions latest available versions collection object
...
```

#### <a name="apidoc.element.npm-check-updates.version_util.colorizeDiff"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>colorizeDiff (strToColor, strToCompare, options)](#apidoc.element.npm-check-updates.version_util.colorizeDiff)
- description and source-code
```javascript
function colorizeDiff(strToColor, strToCompare, options) {

    options = options || {};
    options.color = options.color || 'green';
    var leadingWildcard = '';

    // separate out leading ^ or ~
    if (/^[~^]/.test(strToColor) && strToColor[0] === strToCompare[0]) {
        leadingWildcard = strToColor[0];
        strToColor = strToColor.slice(1);
        strToCompare = strToCompare.slice(1);
    }

    // split into parts
    var partsToColor = strToColor.split('.');
    var partsToCompare = strToCompare.split('.');

    var i = _.findIndex(partsToColor, function (part, i) {
        return part !== partsToCompare[i];
    });
    i = i >= 0 ? i : partsToColor.length;

    // if we are colorizing only part of the word, add a dot in the middle
    var middot = i > 0 && i < partsToColor.length ? '.' : '';

    return leadingWildcard +
        partsToColor.slice(0,i).join('.') +
        middot +
        chalk[options.color](partsToColor.slice(i).join('.'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.version_util.findGreatestByLevel"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>findGreatestByLevel (versions, current, level)](#apidoc.element.npm-check-updates.version_util.findGreatestByLevel)
- description and source-code
```javascript
function findGreatestByLevel(versions, current, level) {
    if (!SEMANTIC_DIRECT.test(current)) {
        return null;
    }

    var cur = semverutils.parse(current);
    return _.chain(versions)
        .map(function (v) {
            return {
                string: v,
                parsed: semverutils.parse(v)
            };
        })
        .filter(function (o) {
            if (level === 'minor' && o.parsed.major !== cur.major) {
                return false;
            }
            return o.parsed[level] === cur[level];
        })
        .map(function (o) {
            return o.string;
        })
        .last()
        .value();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.version_util.getPrecision"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>getPrecision (version)](#apidoc.element.npm-check-updates.version_util.getPrecision)
- description and source-code
```javascript
function getPrecision(version) {
    var semver = semverutils.parseRange(version)[0];
    // expects VERSION_PARTS to be in correct order
    return _.find(VERSION_PARTS.slice().reverse(), _.propertyOf(semver));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.version_util.isWildCard"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>isWildCard (version)](#apidoc.element.npm-check-updates.version_util.isWildCard)
- description and source-code
```javascript
function isWildCard(version) {
    return WILDCARD_PURE_REGEX.test(version);
}
```
- example usage
```shell
...
if (!latestSemver) {
    return declaration;
}

// return global versionUtil.wildcards immediately
if (options.removeRange) {
    return latestVersion;
} else if (versionUtil.isWildCard(declaration)) {
    return declaration;
}

// parse the declaration
// if multiple ranges, use the semver with the least number of parts
var parsedRange = _(semverutils.parseRange(declaration))
    // semver-utils includes empty entries for the || and - operators. We can remove them completely
...
```

#### <a name="apidoc.element.npm-check-updates.version_util.isWildPart"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>isWildPart (versionPart)](#apidoc.element.npm-check-updates.version_util.isWildPart)
- description and source-code
```javascript
function isWildPart(versionPart) {
    return versionPart === '*' || versionPart === 'x';
}
```
- example usage
```shell
...
/**
 * Chooses version parts between the declared version and the latest.
 * Base parts (major, minor, patch) are only included if they are in the original declaration.
 * Added parts (release, build) are always included. They are only present if we are checking --greatest versions
 * anyway.
*/
function chooseVersion(part) {
    return versionUtil.isWildPart(declaredSemver[part]) ? declaredSemver[part] :
        _.includes(versionUtil.VERSION_BASE_PARTS, part) && declaredSemver[part] ? latestSemver[part] :
        _.includes(versionUtil.VERSION_ADDED_PARTS, part) ? latestSemver[part] :
        undefined;
}

// create a new semver object with major, minor, patch, build, and release parts
var newSemver = cint.toObject(versionUtil.VERSION_PARTS, function (part) {
...
```

#### <a name="apidoc.element.npm-check-updates.version_util.numParts"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>numParts (version)](#apidoc.element.npm-check-updates.version_util.numParts)
- description and source-code
```javascript
function numParts(version) {

    var semver = semverutils.parseRange(version)[0];

    if (!semver) {
        throw new Error(util.format('semverutils.parseRange returned null when trying to parse "%s". This is probably a problem
with the "semver-utils" dependency. Please report an issue at https://github.com/tjunnone/npm-check-updates/issues.', version));
    }

    return _.intersection(VERSION_PARTS, Object.keys(semver)).length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.version_util.precisionAdd"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>precisionAdd (precision, n)](#apidoc.element.npm-check-updates.version_util.precisionAdd)
- description and source-code
```javascript
function precisionAdd(precision, n) {

    if (n === 0) {
        return precision;
    }

    var index = n === 0 ? precision :
        _.includes(VERSION_BASE_PARTS, precision) ? VERSION_BASE_PARTS.indexOf(precision) + n :
        _.includes(VERSION_ADDED_PARTS, precision) ? VERSION_BASE_PARTS.length + n :
        null;

    if (index === null) {
        throw new Error('Invalid precision: ' + precision);
    } else if (!VERSION_PARTS[index]) {
        throw new Error('Invalid precision math' + arguments);
    }

    return VERSION_PARTS[index];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.version_util.setPrecision"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>setPrecision (version, precision)](#apidoc.element.npm-check-updates.version_util.setPrecision)
- description and source-code
```javascript
function setPrecision(version, precision) {
    var semver = semverutils.parseRange(version)[0];
    return stringify(semver, precision);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.version_util.stringify"></a>[function <span class="apidocSignatureSpan">npm-check-updates.version_util.</span>stringify (semver, precision)](#apidoc.element.npm-check-updates.version_util.stringify)
- description and source-code
```javascript
function stringify(semver, precision) {

    // get a list of the parts up until (and including) the given precision
    // or all of them, if no precision is specified
    var parts = precision ? VERSION_PARTS.slice(0, VERSION_PARTS.indexOf(precision)+1) : VERSION_PARTS;

    // pair each part with its delimiter and join together
    return parts
        .filter(function (part) {
            return _.includes(VERSION_BASE_PARTS, precision) || semver[part];
        })
        .map(function (part) {
            return VERSION_PART_DELIM[part] + (semver[part] || '0');
        })
        .join('');
}
```
- example usage
```shell
...
        undefined;
}

// create a new semver object with major, minor, patch, build, and release parts
var newSemver = cint.toObject(versionUtil.VERSION_PARTS, function (part) {
    return cint.keyValue(part, chooseVersion(part));
});
var newSemverString = versionUtil.stringify(newSemver);
var version = v(declaredSemver.semver) + newSemverString;

// determine the operator
// do not compact, because [undefined, '<'] must be differentiated from ['<']
var uniqueOperators = _(parsedRange)
    .map(function (range) {
        return range.operator;
...
```



# <a name="apidoc.module.npm-check-updates.versionmanager"></a>[module npm-check-updates.versionmanager](#apidoc.module.npm-check-updates.versionmanager)

#### <a name="apidoc.element.npm-check-updates.versionmanager.getCurrentDependencies"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getCurrentDependencies (pkgData, options)](#apidoc.element.npm-check-updates.versionmanager.getCurrentDependencies)
- description and source-code
```javascript
function getCurrentDependencies(pkgData, options) {

    pkgData = pkgData || {};
    options = options || {};

    if (!options.prod && !options.dev && !options.optional) {
        options.prod = options.dev = options.optional = true;
    }

    var allDependencies = cint.filterObject(_.merge({},
        options.prod && pkgData.dependencies,
        options.dev && pkgData.devDependencies,
        options.optional && pkgData.optionalDependencies
    ), filterAndReject(options.filter, options.reject));

    return allDependencies;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.getGreatestPackageVersion"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getGreatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.versionmanager.getGreatestPackageVersion)
- description and source-code
```javascript
getGreatestPackageVersion = function (pkgData) {
    return selectedPackageManager.greatest(pkgData);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.getInstalledPackages"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getInstalledPackages (options)](#apidoc.element.npm-check-updates.versionmanager.getInstalledPackages)
- description and source-code
```javascript
function getInstalledPackages(options) {

    options = options || {};

    return selectedPackageManager.list([], {cwd: options.cwd}).then(function (results) {
        if (!results || !results.dependencies) {
            throw new Error('Unable to retrieve NPM package list');
        }

        // filter out undefined packages or those with a wildcard
        var filterFunction = filterAndReject(options.filter, options.reject);
        var validPackages = cint.filterObject(results.dependencies, function (dep, pkgInfo) {
            return pkgInfo && pkgInfo.name && pkgInfo.version && !versionUtil.isWildPart(pkgInfo.version) && filterFunction(dep);
        });

        // convert the dependency object from npm into a simple object that maps the package name to its version
        var simpleDependencies = cint.mapObject(validPackages, function (dep, pkgInfo) {
            return cint.keyValue(dep, pkgInfo.version);
        });

        return simpleDependencies;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.getLatestPackageVersion"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getLatestPackageVersion (pkgData)](#apidoc.element.npm-check-updates.versionmanager.getLatestPackageVersion)
- description and source-code
```javascript
getLatestPackageVersion = function (pkgData) {
    return selectedPackageManager.latest(pkgData);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.getPreferredWildcard"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getPreferredWildcard (dependencies)](#apidoc.element.npm-check-updates.versionmanager.getPreferredWildcard)
- description and source-code
```javascript
function getPreferredWildcard(dependencies) {

    // if there are no dependencies, return null.
    if (Object.keys(dependencies).length === 0) {
        return null;
    }

    // group the dependencies by wildcard
    var groups = _.groupBy(_.values(dependencies), function (dep) {
        return _.find(versionUtil.WILDCARDS, function (wildcard) {
            return dep && dep.indexOf(wildcard) > -1;
        });
    });

    // if none of the dependencies use a wildcard, return null
    var usedWildcards = Object.keys(groups);
    if (usedWildcards.length === 1 && usedWildcards[0] === 'undefined') {
        return null;
    }

    // convert to an array of objects that can be sorted
    var arrOfGroups = cint.toArray(groups, function (wildcard, instances) {
        return {
            wildcard: wildcard,
            instances: instances
        };
    });

    // reverse sort the groups so that the wildcard with the most appearances is at the head, then return it.
    var sorted = _.sortBy(arrOfGroups, function (wildcardObject) {
        return -wildcardObject.instances.length;
    });

    return sorted[0].wildcard;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.getVersionTarget"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>getVersionTarget (options)](#apidoc.element.npm-check-updates.versionmanager.getVersionTarget)
- description and source-code
```javascript
function getVersionTarget(options) {
    return options.semverLevel ? options.semverLevel :
        options.newest ? 'newest' :
        options.greatest ? 'greatest' :
        'latest';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.initialize"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>initialize (args)](#apidoc.element.npm-check-updates.versionmanager.initialize)
- description and source-code
```javascript
function initialize(args) {

    args = args || {};
    args.packageManager = args.packageManager || 'npm';

    if (!(args.packageManager in packageManagers)) {
        throw new Error('Invalid package manager: ' + args.packageManager);
    }

    selectedPackageManager = packageManagers[args.packageManager];

    return selectedPackageManager.init({
        global: args.global,
        registry: args.registry
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.isSatisfied"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>isSatisfied (version, range, loose)](#apidoc.element.npm-check-updates.versionmanager.isSatisfied)
- description and source-code
```javascript
function satisfies(version, range, loose) {
  try {
    range = new Range(range, loose);
  } catch (er) {
    return false;
  }
  return range.test(version);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.isUpgradeable"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>isUpgradeable (current, latest)](#apidoc.element.npm-check-updates.versionmanager.isUpgradeable)
- description and source-code
```javascript
function isUpgradeable(current, latest) {

    // do not upgrade non-npm version declarations (such as git tags)
    // do not upgrade versionUtil.wildcards
    if (!semver.validRange(current) || versionUtil.isWildCard(current)) {
        return false;
    }

    // remove the constraint (e.g. ^1.0.1 -> 1.0.1) to allow upgrades that satisfy the range, but are out of date
    var range = semverutils.parseRange(current)[0];
    if (!range) {
        throw new Error('"' + current + '" could not be parsed by semver-utils. This is probably a bug. Please file an issue at
https://github.com/tjunnone/npm-check-updates.');
    }
    var version = versionUtil.stringify(range);

    // make sure it is a valid range
    // not upgradeable if the latest version satisfies the current range
    // not upgradeable if the specified version is newer than the latest (indicating a prerelease version)
    return Boolean(semver.validRange(version)) &&
        !isSatisfied(latest, version) &&
        !semver.ltr(latest, version);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.queryVersions"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>queryVersions (packageMap, options)](#apidoc.element.npm-check-updates.versionmanager.queryVersions)
- description and source-code
```javascript
function queryVersions(packageMap, options) {

    var getPackageVersion;
    options = options || {};

    var packageList = Object.keys(packageMap);

    // validate options.versionTarget
    options.versionTarget = options.versionTarget || 'latest';

    // determine the getPackageVersion function from options.versionTarget
    switch (options.versionTarget) {
        case 'latest':
            getPackageVersion = selectedPackageManager.latest;
            break;
        case 'greatest':
            getPackageVersion = selectedPackageManager.greatest;
            break;
        case 'newest':
            getPackageVersion = selectedPackageManager.newest;
            break;
        case 'major':
            getPackageVersion = selectedPackageManager.greatestMajor;
            break;
        case 'minor':
            getPackageVersion = selectedPackageManager.greatestMinor;
            break;
        default:
            var supportedVersionTargets = ['latest', 'newest', 'greatest', 'major', 'minor'];
            return Promise.reject(new Error('Unsupported versionTarget: ' + options.versionTarget +
                '. Supported version targets are: ' + supportedVersionTargets.join(', ')));
    }

    // ignore 404 errors from getPackageVersion by having them return null instead of rejecting
    function getPackageVersionProtected(dep) {
        return getPackageVersion(dep, packageMap[dep]).catch(function (err) {
            if (err.message == 404) { // eslint-disable-line eqeqeq
                return null;
            } else {
                throw err;
            }
        });
    }

    // zip up the array of versions into to a nicer object keyed by package name
    function zipVersions(versionList) {
        return cint.toObject(versionList, function (version, i) {
            return cint.keyValue(packageList[i], version);
        });
    }

    return Promise.map(packageList, getPackageVersionProtected)
        .then(zipVersions)
        .then(_.partialRight(_.pickBy, _.identity));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.upgradeDependencies"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradeDependencies (currentDependencies, latestVersions, options)](#apidoc.element.npm-check-updates.versionmanager.upgradeDependencies)
- description and source-code
```javascript
function upgradeDependencies(currentDependencies, latestVersions, options) {

    options = options || {};

    // filter out dependencies with empty values
    currentDependencies = cint.filterObject(currentDependencies, function (key, value) {
        return value;
    });

    // get the preferred wildcard and bind it to upgradeDependencyDeclaration
    var wildcard = getPreferredWildcard(currentDependencies) || DEFAULT_WILDCARD;
    var upgradeDep = _.partialRight(upgradeDependencyDeclaration, {
        wildcard: wildcard,
        removeRange: options.removeRange
    });

    return _(currentDependencies)
        // only include packages for which a latest version was fetched
        .pickBy(function (current, packageName) {
            return packageName in latestVersions;
        })
        // combine the current and latest dependency objects into a single object keyed by packageName and containing
        // both versions in an array: [current, latest]
        .mapValues(function (current, packageName) {
            var latest = latestVersions[packageName];
            return [current, latest];
        })
        // pick the packages that are upgradeable
        // we can use spread because isUpgradeable and upgradeDependencyDeclaration both take current and latest as
        // arguments
        .pickBy(_.spread(isUpgradeable))
        .mapValues(_.spread(upgradeDep))
        .value();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.upgradeDependencyDeclaration"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradeDependencyDeclaration (declaration, latestVersion, options)](#apidoc.element.npm-check-updates.versionmanager.upgradeDependencyDeclaration)
- description and source-code
```javascript
function upgradeDependencyDeclaration(declaration, latestVersion, options) {

    options = options || {};
    options.wildcard = options.wildcard || DEFAULT_WILDCARD;

    // parse the latestVersion
    // return original declaration if latestSemver is invalid
    var latestSemver = semverutils.parseRange(latestVersion)[0];
    if (!latestSemver) {
        return declaration;
    }

    // return global versionUtil.wildcards immediately
    if (options.removeRange) {
        return latestVersion;
    } else if (versionUtil.isWildCard(declaration)) {
        return declaration;
    }

    // parse the declaration
    // if multiple ranges, use the semver with the least number of parts
    var parsedRange = _(semverutils.parseRange(declaration))
        // semver-utils includes empty entries for the || and - operators. We can remove them completely
        .reject({operator: '||'})
        .reject({operator: '-'})
        .sortBy(_.ary(_.flow(versionUtil.stringify, versionUtil.numParts), 1))
        .value();
    var declaredSemver = parsedRange[0];

<span class="apidocCodeCommentSpan">    /**
     * Chooses version parts between the declared version and the latest.
     * Base parts (major, minor, patch) are only included if they are in the original declaration.
     * Added parts (release, build) are always included. They are only present if we are checking --greatest versions
     * anyway.
    */
</span>    function chooseVersion(part) {
        return versionUtil.isWildPart(declaredSemver[part]) ? declaredSemver[part] :
            _.includes(versionUtil.VERSION_BASE_PARTS, part) && declaredSemver[part] ? latestSemver[part] :
            _.includes(versionUtil.VERSION_ADDED_PARTS, part) ? latestSemver[part] :
            undefined;
    }

    // create a new semver object with major, minor, patch, build, and release parts
    var newSemver = cint.toObject(versionUtil.VERSION_PARTS, function (part) {
        return cint.keyValue(part, chooseVersion(part));
    });
    var newSemverString = versionUtil.stringify(newSemver);
    var version = v(declaredSemver.semver) + newSemverString;

    // determine the operator
    // do not compact, because [undefined, '<'] must be differentiated from ['<']
    var uniqueOperators = _(parsedRange)
        .map(function (range) {
            return range.operator;
        })
        .uniq()
        .value();
    var operator = uniqueOperators[0] || '';

    var hasWildCard = versionUtil.WILDCARDS.some(_.partial(_.includes, newSemverString, _, 0));
    var isLessThan = uniqueOperators[0] === '<' || uniqueOperators[0] === '<=';
    var isMixed = uniqueOperators.length > 1;

    // convert versions with </<= or mixed operators into the preferred wildcard
    // only do so if the new version does not already contain a wildcard
    return !hasWildCard && (isLessThan || isMixed) ?
        versionUtil.addWildCard(version, options.wildcard) :
        operator + version;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.upgradePackageData"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradePackageData (pkgData, oldDependencies, newDependencies, newVersions, options)](#apidoc.element.npm-check-updates.versionmanager.upgradePackageData)
- description and source-code
```javascript
function upgradePackageData(pkgData, oldDependencies, newDependencies, newVersions, options) {

    options = options || {};

    for (var dependency in newDependencies) {
        if (options.upgradeAll || !isSatisfied(newVersions[dependency], oldDependencies[dependency])) {
            var expression = '"' + dependency + '"\\s*:\\s*"' + escapeRegexp(oldDependencies[dependency] + '"');
            var regExp = new RegExp(expression, 'g');
            pkgData = pkgData.replace(regExp, '"' + dependency + '": ' + '"' + newDependencies[dependency] + '"');
        }
    }

    return pkgData;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-check-updates.versionmanager.upgradePackageDefinitions"></a>[function <span class="apidocSignatureSpan">npm-check-updates.versionmanager.</span>upgradePackageDefinitions (currentDependencies, options)](#apidoc.element.npm-check-updates.versionmanager.upgradePackageDefinitions)
- description and source-code
```javascript
function upgradePackageDefinitions(currentDependencies, options) {
    var versionTarget = getVersionTarget(options);

    return queryVersions(currentDependencies, {
        versionTarget: versionTarget,
        registry: options.registry ? options.registry : null
    }).then(function (latestVersions) {

        var upgradedDependencies = upgradeDependencies(currentDependencies, latestVersions, {
            removeRange: options.removeRange
        });

        var filteredUpgradedDependencies = _.pickBy(upgradedDependencies, function (v, dep) {
            return !options.jsonUpgraded || options.upgradeAll || !isSatisfied(latestVersions[dep], currentDependencies[dep]);
        });

        return [filteredUpgradedDependencies, latestVersions];
    });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
