# npm-module-checklist

> Steps to check when starting, working and publishing a module to NPM

[ ] - setup continuous integration server, like [TravisCI][travis] or [CircleCI][circle].

[ ] - run linting and unit tests on each commit locally. [pre-git][pre-git], [ghooks][ghooks]

[ ] - check module published size and white list only necessary files, [tutorial][module size]

[ ] - setup [semantic-release][semantic-release] to automate publishing
and avoid breaking [semver][semver]. This is [important][semver important],
but is currently [broken][broken semver] in too many projects.

[travis]: https://travis-ci.org/
[circle]: https://circleci.com/

[pre-git]: https://github.com/bahmutov/pre-git
[ghooks]: https://www.npmjs.com/package/ghooks

[module size]: http://glebbahmutov.com/blog/smaller-published-NPM-modules/

[semantic-release]: https://github.com/semantic-release/semantic-release
[semver]: http://semver.org/
[semver important]: https://medium.com/javascript-scene/software-versions-are-broken-3d2dc0da0783#.h96ppopx3
[broken semver]: https://www.youtube.com/watch?v=tc2UgG5L7WM

### Small print

Author: Gleb Bahmutov &copy; 2015

* [@bahmutov](https://twitter.com/bahmutov)
* [glebbahmutov.com](http://glebbahmutov.com)
* [blog](http://glebbahmutov.com/blog/)

License: MIT - do anything with the code, but don't blame me if it does not work.

Spread the word: tweet, star on github, etc.

Support: if you find any problems with this module, email / tweet /
[open issue](https://github.com/bahmutov/npm-module-checklist/issues) on Github
