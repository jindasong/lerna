# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

<a name="3.0.0-rc.0"></a>
# [3.0.0-rc.0](https://github.com/lerna/lerna/compare/v3.0.0-beta.21...v3.0.0-rc.0) (2018-07-27)


### Bug Fixes

* **core/package:** Serialize hosted git URLs with original protocol/shorthand ([60ff432](https://github.com/lerna/lerna/commit/60ff432)), closes [#1499](https://github.com/lerna/lerna/issues/1499)
* **publish:** Add default description 'npm' for --npm-client ([649048c](https://github.com/lerna/lerna/commit/649048c))
* **publish:** Avoid fs-extra warning on 32-bit machines ([e908d23](https://github.com/lerna/lerna/commit/e908d23))
* **publish:** Do not leave unstaged changes with --skip-git ([2d497ed](https://github.com/lerna/lerna/commit/2d497ed))
* **publish:** Exit early when publishing w/o commits ([#1453](https://github.com/lerna/lerna/issues/1453)) ([6cbae35](https://github.com/lerna/lerna/commit/6cbae35)), closes [#773](https://github.com/lerna/lerna/issues/773)
* **publish:** Pass --repo-version argument through semver.valid() ([272e9f1](https://github.com/lerna/lerna/commit/272e9f1)), closes [#1483](https://github.com/lerna/lerna/issues/1483)
* **publish:** Update lerna.json version after root preversion lifecycle ([7b3817c](https://github.com/lerna/lerna/commit/7b3817c)), closes [#1495](https://github.com/lerna/lerna/issues/1495)


### Code Refactoring

* **collect-updates:** Make argument signature explicit ([e6ba19f](https://github.com/lerna/lerna/commit/e6ba19f))


### Features

* Add description from --help summary [skip ci] ([9b65d8e](https://github.com/lerna/lerna/commit/9b65d8e))
* **cli:** Upgrade to Yargs 12 ([7899ab8](https://github.com/lerna/lerna/commit/7899ab8))
* **command:** Remove .defaultOptions() from option resolution stack ([2b27a54](https://github.com/lerna/lerna/commit/2b27a54))
* Count packages affected in command summary logging ([5f5e585](https://github.com/lerna/lerna/commit/5f5e585))
* **publish:** Add --require-scripts option to opt-in to raw JS lifecycle scripts ([054392b](https://github.com/lerna/lerna/commit/054392b))
* **publish:** Add `--amend` flag ([#1422](https://github.com/lerna/lerna/issues/1422)) ([ef5f0db](https://github.com/lerna/lerna/commit/ef5f0db))
* **publish:** Ensure published packages contain a LICENSE file ([#1465](https://github.com/lerna/lerna/issues/1465)) ([5863564](https://github.com/lerna/lerna/commit/5863564)), closes [#1213](https://github.com/lerna/lerna/issues/1213)


### BREAKING CHANGES

* **publish:** External `$PKGDIR/scripts/{pre,post}publish.js` lifecycles are now opt-in instead of automatic. Pass `--require-scripts` explicitly to restore previous functionality.
* **collect-updates:** Instead of an opaque command instance, distinct positional arguments are required.





<a name="3.0.0-beta.21"></a>
# [3.0.0-beta.21](https://github.com/lerna/lerna/compare/v3.0.0-beta.20...v3.0.0-beta.21) (2018-05-12)

**Note:** Version bump only for package @lerna/publish





<a name="3.0.0-beta.20"></a>
# [3.0.0-beta.20](https://github.com/lerna/lerna/compare/v3.0.0-beta.19...v3.0.0-beta.20) (2018-05-07)

**Note:** Version bump only for package @lerna/publish





<a name="3.0.0-beta.19"></a>
# [3.0.0-beta.19](https://github.com/lerna/lerna/compare/v3.0.0-beta.18...v3.0.0-beta.19) (2018-05-03)


### Bug Fixes

* **publish:** Include all packages during global major bump ([#1391](https://github.com/lerna/lerna/issues/1391)) ([9cebed1](https://github.com/lerna/lerna/commit/9cebed1)), closes [#1383](https://github.com/lerna/lerna/issues/1383)





<a name="3.0.0-beta.18"></a>
# [3.0.0-beta.18](https://github.com/lerna/lerna/compare/v3.0.0-beta.17...v3.0.0-beta.18) (2018-04-24)


### Bug Fixes

* **git-utils:** Pass `--follow-tags` to `git push` ([6907e90](https://github.com/lerna/lerna/commit/6907e90))


### Features

* **command:** Move GitUtilities.isInitialized into class method ([abecfcc](https://github.com/lerna/lerna/commit/abecfcc))
* **git-utils:** Devolve getCurrentSHA() to consumers ([ecbc1d3](https://github.com/lerna/lerna/commit/ecbc1d3))
* **git-utils:** Devolve getShortSHA() to consumers ([95d179d](https://github.com/lerna/lerna/commit/95d179d))
* **publish:** Move publish-only git utilities ([5594749](https://github.com/lerna/lerna/commit/5594749))


### BREAKING CHANGES

* **git-utils:** Don't use GitUtilities!
* **git-utils:** Don't use GitUtilities.
* **command:** GitUtilities.isInitialized no longer exists. You shouldn't be using GitUtilities.
* **publish:** Many named exports of GitUtilities are no longer provided. Don't use GitUtilities, it's a bad pattern.





<a name="3.0.0-beta.17"></a>
# [3.0.0-beta.17](https://github.com/lerna/lerna/compare/v3.0.0-beta.16...v3.0.0-beta.17) (2018-04-13)

**Note:** Version bump only for package @lerna/publish





<a name="3.0.0-beta.15"></a>
# [3.0.0-beta.15](https://github.com/lerna/lerna/compare/v3.0.0-beta.14...v3.0.0-beta.15) (2018-04-09)


### Features

* **conventional-commits:** Support local file presets ([a1bff40](https://github.com/lerna/lerna/commit/a1bff40))





<a name="3.0.0-beta.14"></a>
# [3.0.0-beta.14](https://github.com/lerna/lerna/compare/v3.0.0-beta.13...v3.0.0-beta.14) (2018-04-03)


### Bug Fixes

* **publish:** Ensure optionalDependencies are updated during publish to registry ([559b731](https://github.com/lerna/lerna/commit/559b731))





<a name="3.0.0-beta.13"></a>
# [3.0.0-beta.13](https://github.com/lerna/lerna/compare/v3.0.0-beta.12...v3.0.0-beta.13) (2018-03-31)


### Features

* Enable progress bars only when necessary ([b766c83](https://github.com/lerna/lerna/commit/b766c83))





<a name="3.0.0-beta.12"></a>
# [3.0.0-beta.12](https://github.com/lerna/lerna/compare/v3.0.0-beta.11...v3.0.0-beta.12) (2018-03-30)


### Features

* **package:** Add `serialize()` method ([fdec3ac](https://github.com/lerna/lerna/commit/fdec3ac))
* **package:** Add Map-like get/set methods, remove raw json getter ([707d1f0](https://github.com/lerna/lerna/commit/707d1f0))
* **project:** Merge `package` and `packageJson` into `manifest` ([9a47ff7](https://github.com/lerna/lerna/commit/9a47ff7))


### BREAKING CHANGES

* **package:** The `Package` class no longer provides direct access to the JSON object
used to construct the instance. Map-like `get()`/`set(val)` methods are
available to modify the internal representation.





<a name="3.0.0-beta.11"></a>
# [3.0.0-beta.11](https://github.com/lerna/lerna/compare/v3.0.0-beta.10...v3.0.0-beta.11) (2018-03-29)


### Bug Fixes

* **publish:** Write temporary annotations once, not repeatedly ([6abae76](https://github.com/lerna/lerna/commit/6abae76))


### Features

* Execute atomic publish lifecycle during lerna publish ([#1348](https://github.com/lerna/lerna/issues/1348)) ([45efa24](https://github.com/lerna/lerna/commit/45efa24))
* Support `optionalDependencies` ([b73e19d](https://github.com/lerna/lerna/commit/b73e19d)), closes [#121](https://github.com/lerna/lerna/issues/121)





<a name="3.0.0-beta.10"></a>
# [3.0.0-beta.10](https://github.com/lerna/lerna/compare/v3.0.0-beta.9...v3.0.0-beta.10) (2018-03-27)


### Features

* **commands:** Delay require of command instantiation ([a1284f3](https://github.com/lerna/lerna/commit/a1284f3))


### BREAKING CHANGES

* **commands:** The default export of command packages is now a factory, not the subclass (which is now a named export).





<a name="3.0.0-beta.9"></a>
# [3.0.0-beta.9](https://github.com/lerna/lerna/compare/v3.0.0-beta.8...v3.0.0-beta.9) (2018-03-24)


### Bug Fixes

* **publish:** Split `--skip-*` properly, leave working tree clean ([5b4b2c9](https://github.com/lerna/lerna/commit/5b4b2c9))


### Features

* **command:** Rename this.repository -> this.project ([43e98a0](https://github.com/lerna/lerna/commit/43e98a0))
* **project:** Use cosmiconfig to locate and read lerna.json ([b8c2789](https://github.com/lerna/lerna/commit/b8c2789))


### BREAKING CHANGES

* **publish:** Previously, gitHead annotations were leftover if `--skip-npm` was passed,
despite no actual requirement for that property when no publishing is going on.

Now, all publish-related operations are truly skipped with `--skip-npm`,
and all git commit/push-related operations are skipped with `--skip-git`.
Passing `--skip-npm` will now also always push to remote, which represents
a breaking change from 2.x behavior.

Thanks @KingScooty for raising the issue!





<a name="3.0.0-beta.8"></a>
# [3.0.0-beta.8](https://github.com/lerna/lerna/compare/v3.0.0-beta.7...v3.0.0-beta.8) (2018-03-22)


### Features

* **utils:** Add "vendored" npm-conf ([9c24a25](https://github.com/lerna/lerna/commit/9c24a25))





<a name="3.0.0-beta.7"></a>
# [3.0.0-beta.7](https://github.com/lerna/lerna/compare/v3.0.0-beta.6...v3.0.0-beta.7) (2018-03-20)

**Note:** Version bump only for package @lerna/publish





<a name="3.0.0-beta.4"></a>
# [3.0.0-beta.4](https://github.com/lerna/lerna/compare/v3.0.0-beta.3...v3.0.0-beta.4) (2018-03-19)

**Note:** Version bump only for package @lerna/publish





<a name="3.0.0-beta.3"></a>
# [3.0.0-beta.3](https://github.com/lerna/lerna/compare/v3.0.0-beta.2...v3.0.0-beta.3) (2018-03-15)


### Features

* Check for upstream changes before attempting to publish ([#1317](https://github.com/lerna/lerna/issues/1317)) ([cef0a69](https://github.com/lerna/lerna/commit/cef0a69))
* Upstream changes warn in CI, throw locally ([4de055d](https://github.com/lerna/lerna/commit/4de055d)), closes [#1177](https://github.com/lerna/lerna/issues/1177) [#1317](https://github.com/lerna/lerna/issues/1317)
* **publish:** Add logging when `--skip-git` or `--skip-npm` are passed ([#1319](https://github.com/lerna/lerna/issues/1319)) ([8eef9ff](https://github.com/lerna/lerna/commit/8eef9ff))





<a name="3.0.0-beta.2"></a>
# [3.0.0-beta.2](https://github.com/lerna/lerna/compare/v3.0.0-beta.1...v3.0.0-beta.2) (2018-03-10)

**Note:** Version bump only for package @lerna/publish





<a name="3.0.0-beta.1"></a>
# [3.0.0-beta.1](https://github.com/lerna/lerna/compare/v3.0.0-beta.0...v3.0.0-beta.1) (2018-03-09)


### Bug Fixes

* **publish:** Checkout manifest changes serially ([ce4a4b1](https://github.com/lerna/lerna/commit/ce4a4b1))
* **publish:** default root manifest name when missing ([a504d7e](https://github.com/lerna/lerna/commit/a504d7e)), closes [#1305](https://github.com/lerna/lerna/issues/1305)
* **publish:** Respect pkg.publishConfig.tag ([04b256a](https://github.com/lerna/lerna/commit/04b256a)), closes [#1311](https://github.com/lerna/lerna/issues/1311)
* **publish:** work around yarn "link:" intransigency ([ddfb517](https://github.com/lerna/lerna/commit/ddfb517)), closes [npm/npm#15900](https://github.com/npm/npm/issues/15900) [yarnpkg/yarn#4212](https://github.com/yarnpkg/yarn/issues/4212)
