# npm-module-checklist
> Steps to check when starting, working and publishing a module to NPM

You can [add](https://github.com/bahmutov/update-markdown) 
the included [CHECKLIST.md](CHECKLIST.md) into your project,
or copy it into your README.md; then check items off as you go.

## Checklist

- [ ] watch the [egghead.io][egghead] series [How to Write an Open Source JavaScript Library][egghead series];
it is extremely useful for any NPM project (OSS or closed-sourced).
- [ ] start unit testing right away, [pick your unit testing framework][pick testing framework]
- [ ] start linting code to prevent obvious problems, like misspelled variable. 
[eslint][eslint], [jshint][jshint], [jscs][jscs] or all of them together 
[gulp-lint-everything][gulp-lint-everything]
- [ ] run linting and unit tests on each commit locally. [pre-git][pre-git], [ghooks][ghooks]
- [ ] validate commit message using [pre-git][pre-git] or [commitizen][commitizen] with [validate-commit-msg][validate-commit-msg]. This
enables other tools, like intelligent release notes.
- [ ] show the project&#39;s GitHub open issues on demand or on commit using [git-issues][git-issues]
- [ ] setup continuous integration server, like [TravisCI][travis] or [CircleCI][circle] (or wait until you set up [semantic-release][semantic-release] which will set up [TravisCI][travis] for you).
- [ ] [add badges][badges] to the README to make broken unit tests or out of date dependencies visible
 - ci server badge
 - published NPM package info
 - production and dev dependencies being out of date
 - semantic release badge
- [ ] check module published size and white list only necessary files, [tutorial][module size]
- [ ] setup [semantic-release][semantic-release] to automate publishing
and avoid breaking [semver][semver]. This is [important][semver important],
but is currently [broken][broken semver] in too many projects. Even this checklist is using semver!
- [ ] avoid surprizes by using exact versions of the top level dependencies. 
Use [save-exact][save-exact] NPM setting and [exact-semver][exact-semver] to enforce it.
- [ ] setup a script to reliably update out of date dependencies using [next-update][next-update install]
- [ ] catch missing or invalid `package.json` values using [grunt-nice-package][grunt-nice-package] 
or [fixpack][fixpack]

Source: [npm-module-checklist](https://github.com/bahmutov/npm-module-checklist)

## Contributors

- Kent C. Dodds [@kentcdodds](https://github.com/kentcdodds)
- Gleb Bahmutov [@bahmutov](https://github.com/bahmutov)

### Small print
Author: Gleb Bahmutov &copy; 2015


- [@bahmutov](https://twitter.com/bahmutov)
- [glebbahmutov.com](http://glebbahmutov.com)
- [blog](http://glebbahmutov.com/blog/)

License: MIT - do anything with the code, but don&#39;t blame me if it does not work.

Spread the word: tweet, star on github, etc.

Support: if you find any problems with this module, email / tweet /
[open issue](https://github.com/bahmutov/npm-module-checklist/issues) on Github

