# Changelog

## 1.0.0 (2026-10-13)


### ⚠ BREAKING CHANGES

* Prefer symlink property set on Vinyl object over its path ([#345](https://github.com/FotoVerite/gulp-vinyl-fs/issues/345))
* Avoid error and reflect filesystem stat if futimes not implemented ([#341](https://github.com/FotoVerite/gulp-vinyl-fs/issues/341))
* Consider the greater of ctime & mtime when comparing since option ([#340](https://github.com/FotoVerite/gulp-vinyl-fs/issues/340))
* Normalize repository, dropping node <10.13 support
* Switch stream implementation to streamx ([#333](https://github.com/FotoVerite/gulp-vinyl-fs/issues/333))

### Features

* Consider the greater of ctime & mtime when comparing since option ([#340](https://github.com/FotoVerite/gulp-vinyl-fs/issues/340)) ([9f907ba](https://github.com/FotoVerite/gulp-vinyl-fs/commit/9f907ba92c71b336b5f82be3881b72328bcea4d7))
* Convert Windows-style paths in `src()` to proper globs ([910c8a5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))
* Prefer symlink property set on Vinyl object over its path ([#345](https://github.com/FotoVerite/gulp-vinyl-fs/issues/345)) ([0ac27a2](https://github.com/FotoVerite/gulp-vinyl-fs/commit/0ac27a284e9e02530b1865b2574c03943cec7446))
* Replace lazystream with streamx Composer ([#344](https://github.com/FotoVerite/gulp-vinyl-fs/issues/344)) ([a80dae3](https://github.com/FotoVerite/gulp-vinyl-fs/commit/a80dae30d7fb1c0f51acc00170648792f740b54b))
* Switch stream implementation to streamx ([#333](https://github.com/FotoVerite/gulp-vinyl-fs/issues/333)) ([910c8a5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))
* Test against streams from core, streamx, and readable-stream ([910c8a5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))


### Bug Fixes

* Add regression test for negative relative globs ([#343](https://github.com/FotoVerite/gulp-vinyl-fs/issues/343)) ([ebe6498](https://github.com/FotoVerite/gulp-vinyl-fs/commit/ebe6498124294306a7491958aebf0d3a184bdf11))
* Additional refactor & tons of tests for metadata update ([6ad732d](https://github.com/FotoVerite/gulp-vinyl-fs/commit/6ad732da5a8bac7c9130a2ee5c632407d2693e14))
* Adjust realMode method to avoid gid in the parse (fixes [#103](https://github.com/FotoVerite/gulp-vinyl-fs/issues/103)) ([7be0cfd](https://github.com/FotoVerite/gulp-vinyl-fs/commit/7be0cfd505aa9cb027d7958814fbd39d37753daf))
* Allow sink to fire readable event on the underlying stream ([9b6a0e2](https://github.com/FotoVerite/gulp-vinyl-fs/commit/9b6a0e2e9d37f666fa58af84348c5592b909b4a1))
* Attempt to fix "write after end" with duplexer2 (closes [#25](https://github.com/FotoVerite/gulp-vinyl-fs/issues/25)) ([d613385](https://github.com/FotoVerite/gulp-vinyl-fs/commit/d613385d4c1fc127c38f81fed92f7c84b8c976ac))
* Attempt to fix "write after end" with un-ending stream (ref [#25](https://github.com/FotoVerite/gulp-vinyl-fs/issues/25)) ([af1b864](https://github.com/FotoVerite/gulp-vinyl-fs/commit/af1b864c35ce8183b533b737c89104f094549273))
* Avoid `file.isDirectory` in `useJunctions` default (fixes [#247](https://github.com/FotoVerite/gulp-vinyl-fs/issues/247)) ([#252](https://github.com/FotoVerite/gulp-vinyl-fs/issues/252)) ([a741486](https://github.com/FotoVerite/gulp-vinyl-fs/commit/a741486930736f0d7d950670227375a5f3e89c79))
* Avoid error and reflect filesystem stat if futimes not implemented ([#341](https://github.com/FotoVerite/gulp-vinyl-fs/issues/341)) ([9ba20fd](https://github.com/FotoVerite/gulp-vinyl-fs/commit/9ba20fd04a6c3a0f191134d60ea6c525259fa237))
* Avoid globbing before read stream is opened ([#362](https://github.com/FotoVerite/gulp-vinyl-fs/issues/362)) ([a13a79a](https://github.com/FotoVerite/gulp-vinyl-fs/commit/a13a79ae67beecf32d0121153a08333bae69fa17))
* Avoid node internals for our WriteStream (fixes [#295](https://github.com/FotoVerite/gulp-vinyl-fs/issues/295)) ([167d8ff](https://github.com/FotoVerite/gulp-vinyl-fs/commit/167d8ffdcbbade502ba3175d3e224fa83ea830e0))
* Avoid Node.js deprecation warning for `fs.Stats` ([#358](https://github.com/FotoVerite/gulp-vinyl-fs/issues/358)) ([3ed0c3f](https://github.com/FotoVerite/gulp-vinyl-fs/commit/3ed0c3f104fec5f05ffc68f198fdc0aae7a68efe))
* Avoid passing `read` option from `src()` to `through2` ([8867645](https://github.com/FotoVerite/gulp-vinyl-fs/commit/8867645b40f70abb297a2a1f45a291f49e53db2b))
* Avoid setting a position in custom write stream (fixes [#202](https://github.com/FotoVerite/gulp-vinyl-fs/issues/202)) ([#203](https://github.com/FotoVerite/gulp-vinyl-fs/issues/203)) ([81f343b](https://github.com/FotoVerite/gulp-vinyl-fs/commit/81f343bb42ece9c1bf249ab8bf26751985bd3104))
* Avoid transcoding streaming output with default options ([#360](https://github.com/FotoVerite/gulp-vinyl-fs/issues/360)) ([7b6dcd3](https://github.com/FotoVerite/gulp-vinyl-fs/commit/7b6dcd3561cee6cae2e90ae9096cb1ca31953db5))
* Avoid TypeError when the `sourcemaps` option is a boolean for `dest()` ([18e8a06](https://github.com/FotoVerite/gulp-vinyl-fs/commit/18e8a061ce73ea21b2ecaac840aceeb74915933c))
* Call the correct callback within symlink (fixes [#298](https://github.com/FotoVerite/gulp-vinyl-fs/issues/298)) ([#299](https://github.com/FotoVerite/gulp-vinyl-fs/issues/299)) ([13390dd](https://github.com/FotoVerite/gulp-vinyl-fs/commit/13390dd8a0b3c2dfa555c89d43241f3385e4aa53))
* Compare modes correctly ([62d2074](https://github.com/FotoVerite/gulp-vinyl-fs/commit/62d2074e782c270a264ed47c2735064b5a5bc1ff))
* Correct regression with src using arrays of globs ([#342](https://github.com/FotoVerite/gulp-vinyl-fs/issues/342)) ([5659934](https://github.com/FotoVerite/gulp-vinyl-fs/commit/565993435f9d15712ade3c7c422030d3022f3742))
* Depend on process default mode for new files/directories ([986b712](https://github.com/FotoVerite/gulp-vinyl-fs/commit/986b71200b96327d647743c2d2ad230ccee316dd))
* Determine symlink type for directory symlinks on Windows (closes [#74](https://github.com/FotoVerite/gulp-vinyl-fs/issues/74)) ([949ebbe](https://github.com/FotoVerite/gulp-vinyl-fs/commit/949ebbeb0eb7902b27f1c74248585e309a8cadcf))
* Don't rely on undocumented Stream.fd property ([#175](https://github.com/FotoVerite/gulp-vinyl-fs/issues/175)) ([c7798bb](https://github.com/FotoVerite/gulp-vinyl-fs/commit/c7798bb64b2c92212a2cc4e2f18c81d4e124ad49))
* Ensure `atime` is a Date object ([e9584ce](https://github.com/FotoVerite/gulp-vinyl-fs/commit/e9584ceb8b718b53d5995168182f0a1434676cc0))
* Get writeStream working ([8b28778](https://github.com/FotoVerite/gulp-vinyl-fs/commit/8b28778bc232fc1dea432d720d86b0e41318da14))
* Ignore atime/mtime if they are invalid (fixes [#113](https://github.com/FotoVerite/gulp-vinyl-fs/issues/113)) ([86492a7](https://github.com/FotoVerite/gulp-vinyl-fs/commit/86492a7577e480680bbe315a5d3ef144bf2fdb11))
* Improve sink implementation ([feb1270](https://github.com/FotoVerite/gulp-vinyl-fs/commit/feb1270ee2483d69d10aa260f205c2eddc8c56f6))
* Improve sourcemap handling ([b96497a](https://github.com/FotoVerite/gulp-vinyl-fs/commit/b96497a5c1240a9d95cd89d0357467eec201b5e2))
* Improve stats logic to avoid problems when files not owned ([559c2d5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/559c2d5dc55bdfad31045ed8543cb4c396146a0a))
* Improve symlink following logic for correct `file.base` in `src()` (fixes [#132](https://github.com/FotoVerite/gulp-vinyl-fs/issues/132)) ([a1d4ccc](https://github.com/FotoVerite/gulp-vinyl-fs/commit/a1d4cccfa5213ed78de3a1a16924fedb036e37d4))
* Improve/refactor metadata handling & fix tests ([b7cb0f0](https://github.com/FotoVerite/gulp-vinyl-fs/commit/b7cb0f0aa762c1f6f4e1388897bab9e4acbbb070))
* Include the invalid glob in error message ([2727071](https://github.com/FotoVerite/gulp-vinyl-fs/commit/2727071fa8cdb4428745005666738b3e3e78c26f))
* Increase offset in futimes test timestamps ([#176](https://github.com/FotoVerite/gulp-vinyl-fs/issues/176)) ([12f92f8](https://github.com/FotoVerite/gulp-vinyl-fs/commit/12f92f884e79098d4e9e9e8a71e4aaa7212deda4))
* Make tests aware of umask & use octal strings for expected results (fixes [#166](https://github.com/FotoVerite/gulp-vinyl-fs/issues/166)) ([31b0a66](https://github.com/FotoVerite/gulp-vinyl-fs/commit/31b0a66064e4c65eb676b1c4ed67bfb13f764c27))
* Pin gulp-sourcemaps to avoid breaking changes ([63808d8](https://github.com/FotoVerite/gulp-vinyl-fs/commit/63808d814ea8d9a34e17d766ee63d21fa7ee369e))
* Propagate errors during symlink prepareWrite ([712a0c5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/712a0c5dfb1c4877ba554af406e969f70d95a925))
* Properly handle file in mkdirp path (closes [#181](https://github.com/FotoVerite/gulp-vinyl-fs/issues/181)) ([3087b78](https://github.com/FotoVerite/gulp-vinyl-fs/commit/3087b78038e01a27e5047029328afee6afb55481))
* Re-emit errors on output stream to propagate singular glob errors ([efd4139](https://github.com/FotoVerite/gulp-vinyl-fs/commit/efd413904eec760d4d1c1b6b0cb05523ad4e4b57))
* Refactor writeStream to prevent issue with futimes ([bdbe46d](https://github.com/FotoVerite/gulp-vinyl-fs/commit/bdbe46df033beca7a5666f70215d82d0894ebe05))
* Reference correct property name in integration testing ([#320](https://github.com/FotoVerite/gulp-vinyl-fs/issues/320)) ([df245a4](https://github.com/FotoVerite/gulp-vinyl-fs/commit/df245a40f5dbe37ca620ee71f1a7930cfccb5e42))
* Remove correct handlers to avoid memory leak ([d370714](https://github.com/FotoVerite/gulp-vinyl-fs/commit/d37071443bb4f37ac089457f8942358360ff9a6b))
* Remove invalid `sourcemaps` option passed to gulp-sourcemaps ([f3242e7](https://github.com/FotoVerite/gulp-vinyl-fs/commit/f3242e7f77ebab6a1b20cfe11a413f71e112ea8f))
* Remove lodash.isequal dependency due to changed behavior ([94f7ac7](https://github.com/FotoVerite/gulp-vinyl-fs/commit/94f7ac70ec55c8ae80bcde3769d7b54ffdf21e7c))
* Remove memory leak when writing streaming contents ([4820c79](https://github.com/FotoVerite/gulp-vinyl-fs/commit/4820c795b4377e5fc990ceb739ced496fa491ee0))
* Replace vinyl-filter-since with own working implementation ([8e15c49](https://github.com/FotoVerite/gulp-vinyl-fs/commit/8e15c49dc798555ab3cea40b2b03d77ea9edc355))
* Resolve broken refactor problems ([c196935](https://github.com/FotoVerite/gulp-vinyl-fs/commit/c196935e0063264eb217111cf2031d7fee88b107))
* Return an empty stream if empty array is passed to `src()` (closes [#40](https://github.com/FotoVerite/gulp-vinyl-fs/issues/40)) ([8744943](https://github.com/FotoVerite/gulp-vinyl-fs/commit/8744943c9403d586e37757f01a8a8520b025b498))
* Revert string support from previous release & add SlowBuffer support ([49148b8](https://github.com/FotoVerite/gulp-vinyl-fs/commit/49148b8027adb4026905b718d759933b28d29e7f))
* Sink the `dest()` stream by attaching a noop data listener (fixes [#26](https://github.com/FotoVerite/gulp-vinyl-fs/issues/26)) ([7316311](https://github.com/FotoVerite/gulp-vinyl-fs/commit/7316311286d9005638ba036dcf92d4f985a3daaa))
* Sink the saveStream on nextTick to start flowing and avoid highWaterMark ([007aae1](https://github.com/FotoVerite/gulp-vinyl-fs/commit/007aae1510003af3f396ed10a5f857fbc7a8ed46))
* Skip broken tests that were false positives ([b552beb](https://github.com/FotoVerite/gulp-vinyl-fs/commit/b552beb6a16edca7e93fc5e97dcc8f02025fc345))
* Support setting setuid/setgid/sticky in updateMetadata (fixes [#156](https://github.com/FotoVerite/gulp-vinyl-fs/issues/156)) ([799b057](https://github.com/FotoVerite/gulp-vinyl-fs/commit/799b0570d49c28cca0bd1aab8df4ca3600a680af))
* Support strings in `writeFile` implementation ([453f063](https://github.com/FotoVerite/gulp-vinyl-fs/commit/453f06300ac0dbe09b719a36a7125ff6e737a45e))
* Temporarily marshall old Vinyl objects to latest version in dest/symlink ([#291](https://github.com/FotoVerite/gulp-vinyl-fs/issues/291)) ([bbfb50c](https://github.com/FotoVerite/gulp-vinyl-fs/commit/bbfb50c0311a489fd8238a2cbf9524eac0f6bb04))
* Upgrade glob-stream to remove path.normalize workaround ([8cfb322](https://github.com/FotoVerite/gulp-vinyl-fs/commit/8cfb322d95d54bbce448ec36c8d6c95e6def4818))
* Use `fs.futimes` to retain sub-second precision in `atime`/`mtime` ([4ff0e8d](https://github.com/FotoVerite/gulp-vinyl-fs/commit/4ff0e8d5170b4fe38116aa1b76ee59ea7b26f6b8))
* Use custom implementation of fs.WriteStream that supports flush (fixes [#189](https://github.com/FotoVerite/gulp-vinyl-fs/issues/189)) ([483d1cc](https://github.com/FotoVerite/gulp-vinyl-fs/commit/483d1cca7b60d79817dcbce99e4f465f4b69cb1f))
* Use explicit chmod to ensure setgid permission can be set & account for umask with default mode (closes [#183](https://github.com/FotoVerite/gulp-vinyl-fs/issues/183), closes [#185](https://github.com/FotoVerite/gulp-vinyl-fs/issues/185)) ([8eb33dc](https://github.com/FotoVerite/gulp-vinyl-fs/commit/8eb33dc2ec9b995e001701dd4adc8b02961400e6))
* Use lazystream for streamFile to avoid fd exhaustion ([542771a](https://github.com/FotoVerite/gulp-vinyl-fs/commit/542771ad541df66d0e7ee4254cf3ab3681c72a55))
* Use the sink stream utility to sink symlink stream (closes [#195](https://github.com/FotoVerite/gulp-vinyl-fs/issues/195)) ([7a16a0b](https://github.com/FotoVerite/gulp-vinyl-fs/commit/7a16a0b3beea7a86cebd2758a75f303540788bf8))
* Verify `src()` & `dest()` arguments (closes [#8](https://github.com/FotoVerite/gulp-vinyl-fs/issues/8)) ([15fe287](https://github.com/FotoVerite/gulp-vinyl-fs/commit/15fe287647820b7357530190708cfd00c62dfe8f))
* Workaround symlink stat bug in Node 10 on Windows ([910c8a5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))


### Miscellaneous Chores

* Normalize repository, dropping node &lt;10.13 support ([910c8a5](https://github.com/FotoVerite/gulp-vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))

### [4.0.2](https://www.github.com/gulpjs/vinyl-fs/compare/v4.0.1...v4.0.2) (2025-06-01)


### Bug Fixes

* Avoid globbing before read stream is opened ([#362](https://www.github.com/gulpjs/vinyl-fs/issues/362)) ([a13a79a](https://www.github.com/gulpjs/vinyl-fs/commit/a13a79ae67beecf32d0121153a08333bae69fa17))

### [4.0.1](https://www.github.com/gulpjs/vinyl-fs/compare/v4.0.0...v4.0.1) (2025-06-01)


### Bug Fixes

* Avoid Node.js deprecation warning for `fs.Stats` ([#358](https://www.github.com/gulpjs/vinyl-fs/issues/358)) ([3ed0c3f](https://www.github.com/gulpjs/vinyl-fs/commit/3ed0c3f104fec5f05ffc68f198fdc0aae7a68efe))
* Avoid transcoding streaming output with default options ([#360](https://www.github.com/gulpjs/vinyl-fs/issues/360)) ([7b6dcd3](https://www.github.com/gulpjs/vinyl-fs/commit/7b6dcd3561cee6cae2e90ae9096cb1ca31953db5))

## [4.0.0](https://www.github.com/gulpjs/vinyl-fs/compare/v3.0.3...v4.0.0) (2023-06-11)


### ⚠ BREAKING CHANGES

* Prefer symlink property set on Vinyl object over its path (#345)
* Avoid error and reflect filesystem stat if futimes not implemented (#341)
* Consider the greater of ctime & mtime when comparing since option (#340)
* Normalize repository, dropping node <10.13 support
* Switch stream implementation to streamx (#333)
* Default to `utf8` decoding and encoding. Add `encoding` option to change (#287)

### Features

* Consider the greater of ctime & mtime when comparing since option ([#340](https://www.github.com/gulpjs/vinyl-fs/issues/340)) ([9f907ba](https://www.github.com/gulpjs/vinyl-fs/commit/9f907ba92c71b336b5f82be3881b72328bcea4d7))
* Convert Windows-style paths in `src()` to proper globs ([910c8a5](https://www.github.com/gulpjs/vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))
* Prefer symlink property set on Vinyl object over its path ([#345](https://www.github.com/gulpjs/vinyl-fs/issues/345)) ([0ac27a2](https://www.github.com/gulpjs/vinyl-fs/commit/0ac27a284e9e02530b1865b2574c03943cec7446))
* Replace lazystream with streamx Composer ([#344](https://www.github.com/gulpjs/vinyl-fs/issues/344)) ([a80dae3](https://www.github.com/gulpjs/vinyl-fs/commit/a80dae30d7fb1c0f51acc00170648792f740b54b))
* Switch stream implementation to streamx ([#333](https://www.github.com/gulpjs/vinyl-fs/issues/333)) ([910c8a5](https://www.github.com/gulpjs/vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))
* Test against streams from core, streamx, and readable-stream ([910c8a5](https://www.github.com/gulpjs/vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))
* Default to `utf8` decoding and encoding. Add `encoding` option to change (#287)

### Bug Fixes

* Add regression test for negative relative globs ([#343](https://www.github.com/gulpjs/vinyl-fs/issues/343)) ([ebe6498](https://www.github.com/gulpjs/vinyl-fs/commit/ebe6498124294306a7491958aebf0d3a184bdf11))
* Avoid error and reflect filesystem stat if futimes not implemented ([#341](https://www.github.com/gulpjs/vinyl-fs/issues/341)) ([9ba20fd](https://www.github.com/gulpjs/vinyl-fs/commit/9ba20fd04a6c3a0f191134d60ea6c525259fa237))
* Correct regression with src using arrays of globs ([#342](https://www.github.com/gulpjs/vinyl-fs/issues/342)) ([5659934](https://www.github.com/gulpjs/vinyl-fs/commit/565993435f9d15712ade3c7c422030d3022f3742))
* Reference correct property name in integration testing ([#320](https://www.github.com/gulpjs/vinyl-fs/issues/320)) ([df245a4](https://www.github.com/gulpjs/vinyl-fs/commit/df245a40f5dbe37ca620ee71f1a7930cfccb5e42))
* Workaround symlink stat bug in Node 10 on Windows ([910c8a5](https://www.github.com/gulpjs/vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))


### Miscellaneous Chores

* Normalize repository, dropping node <10.13 support ([910c8a5](https://www.github.com/gulpjs/vinyl-fs/commit/910c8a521834d5aa9dec5a83102b59ba5c531e08))
