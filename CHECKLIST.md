- [ ] watch the [egghead.io][egghead] series [How to Write an Open Source JavaScript Library][egghead series];
it is extremely useful for any NPM project (OSS or closed-sourced).

- [ ] start unit testing right away, [pick your unit testing framework][pick testing framework]

- [ ] start linting code to prevent obvious problems, like misspelled variable.
[eslint][eslint], [jshint][jshint], [jscs][jscs] or all of them together
[gulp-lint-everything][gulp-lint-everything]

- [ ] run linting and unit tests on each commit locally. [pre-git][pre-git], [ghooks][ghooks]

- [ ] validate commit message using [pre-git][pre-git] or [commitizen][commitizen] with [validate-commit-msg][validate-commit-msg]. This
enables other tools, like intelligent release notes.

- [ ] show the project's GitHub open issues on demand or on commit using [git-issues][git-issues]

- [ ] setup continuous integration server, like [TravisCI][travis] or [CircleCI][circle] (or wait until you set up [semantic-release][semantic-release] which will set up [TravisCI][travis] for you).

- [ ] [add badges][badges] to the README to make broken unit tests or out of date dependencies visible
  * ci server badge
  * published NPM package info [NodeICO][nodeico]
  * production and dev dependencies being out of date [david-dm][david-dm]
  * semantic release badge

- [ ] check module published size and white list only necessary files, [tutorial][module size]

- [ ] setup [semantic-release][semantic-release] to automate publishing
and avoid breaking [semver][semver]. This is [important][semver important],
but is currently [broken][broken semver] in too many projects. Even this checklist is using semver!

- [ ] avoid surprizes by using exact versions of the top level dependencies.
Use [save-exact][save-exact] NPM setting and [exact-semver][exact-semver] to enforce it.

- [ ] setup a script to reliably update out of date dependencies using [next-update][next-update install]
  - [ ] setup automatic pull requests when newer versions of dependencies appear [greenkeeper.io][greenkeeper]

- [ ] catch missing or invalid `package.json` values using [grunt-nice-package][grunt-nice-package]
or [fixpack][fixpack]

- [ ] write simple installation commands for your module

- [ ] write "quick intro" example showing the main feature of your module

- [ ] add CONTRIBUTING.md file with clear guidelines how others can add new features or fix bugs
in your module. [Atom editor][atom] and [lodash][lodash] have excellent examples to follow.

- [ ] generate documentation automatically. [xplain][xplain] is my own tool for JS to HTML/Markdown
generation

- [ ] place most of the public API documentation in README file for simple retrieval.
This allows other developers to find relevant sections right from the command line [manpm][manpm]
or by looking up `npm home <package name>`

[egghead]: https://egghead.io
[egghead series]: https://egghead.io/series/how-to-write-an-open-source-javascript-library

[pick testing framework]: http://glebbahmutov.com/blog/picking-javascript-testing-framework/

[eslint]: http://eslint.org/
[jshint]: http://jshint.com/docs/
[jscs]: http://jscs.info/
[gulp-lint-everything]: https://github.com/bahmutov/gulp-lint-everything

[pre-git]: https://github.com/bahmutov/pre-git
[ghooks]: https://www.npmjs.com/package/ghooks

[commitizen]: https://www.npmjs.com/package/commitizen

[validate-commit-msg]: https://www.npmjs.com/package/validate-commit-msg

[git-issues]: https://www.npmjs.com/package/git-issues

[travis]: https://travis-ci.org/
[circle]: https://circleci.com/

[badges]: http://glebbahmutov.com/blog/tightening-node-project/
[nodeico]: https://nodei.co/
[david-dm]: https://david-dm.org/

[module size]: http://glebbahmutov.com/blog/smaller-published-NPM-modules/

[semantic-release]: https://github.com/semantic-release/semantic-release
[semver]: http://semver.org/
[semver important]: https://medium.com/javascript-scene/software-versions-are-broken-3d2dc0da0783#.h96ppopx3
[broken semver]: https://www.youtube.com/watch?v=tc2UgG5L7WM

[save-exact]: https://docs.npmjs.com/misc/config#save-exact
[exact-semver]: https://github.com/bahmutov/exact-semver

[next-update install]: https://github.com/bahmutov/next-update#install
[greenkeeper]: http://greenkeeper.io/

[grunt-nice-package]: https://github.com/bahmutov/grunt-nice-package
[fixpack]: https://github.com/henrikjoreteg/fixpack

[atom]: https://github.com/atom/atom/blob/master/CONTRIBUTING.md
[lodash]: https://github.com/lodash/lodash/blob/master/CONTRIBUTING.md

[xplain]: https://github.com/bahmutov/xplain

[manpm]: https://github.com/bahmutov/manpm

Source: [npm-module-checklist](https://github.com/bahmutov/npm-module-checklist)
