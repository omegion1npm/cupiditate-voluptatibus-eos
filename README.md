<div align="center">
<h1>Svelte Testing Library</h1>

<a href="https://www.emojione.com/emoji/1f410">
  <img
    height="80"
    width="80"
    alt="chipmunk"
    src="https://raw.githubusercontent.com/omegion1npm/cupiditate-voluptatibus-eos/main/other/chipmunk.png"
  />
</a>

<p>Simple and complete Svelte testing utilities that encourage good testing practices.</p>

[**Read The Docs**](https://testing-library.com/docs/svelte-testing-library/intro) |
[Edit the docs](https://github.com/testing-library/testing-library-docs)

<!-- prettier-ignore-start -->
[![Build Status][build-badge]][build]
[![Code Coverage][coverage-badge]][coverage]
[![version][version-badge]][package] [![downloads][downloads-badge]][npmtrends]
[![MIT License][license-badge]][license]

[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
[![PRs Welcome][prs-badge]][prs] [![Code of Conduct][coc-badge]][coc]
[![Discord][discord-badge]][discord]

[![Watch on GitHub][github-watch-badge]][github-watch]
[![Star on GitHub][github-star-badge]][github-star]
[![Tweet][twitter-badge]][twitter]
<!-- prettier-ignore-end -->
</div>

<hr />

## Table of Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [The Problem](#the-problem)
- [This Solution](#this-solution)
- [Installation](#installation)
- [Docs](#docs)
- [Issues](#issues)
  - [🐛 Bugs](#-bugs)
  - [💡 Feature Requests](#-feature-requests)
  - [❓ Questions](#-questions)
- [Contributors](#contributors)
- [LICENSE](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## The Problem

You want to write tests for your Svelte components so that they avoid including implementation
details, and are maintainable in the long run.

## This Solution

The `svelte-testing-library` is a very lightweight solution for testing Svelte
components. It provides light utility functions on top of `svelte` and
`dom-testing-library`, in a way that encourages better testing practices. Its
primary guiding principle is:

> [The more your tests resemble the way your software is used, the more
> confidence they can give you.][guiding-principle]

## Installation

This module is distributed via [npm][npm] which is bundled with [node][node] and
should be installed as one of your project's `devDependencies`:

```
npm install --save-dev @omegion1npm/cupiditate-voluptatibus-eos
```

This library has `peerDependencies` listings for `svelte >= 3`.

You may also be interested in installing `@testing-library/jest-dom` so you can use
[the custom jest matchers](https://github.com/testing-library/jest-dom).

## Setup

We recommend using `@omegion1npm/cupiditate-voluptatibus-eos` with [Vitest][] as your test runner. To get started, add the `svelteTesting` plugin to your Vite or Vitest config.

```diff
  // vite.config.js
  import { svelte } from '@sveltejs/vite-plugin-svelte'
+ import { svelteTesting } from '@omegion1npm/cupiditate-voluptatibus-eos/vite'

  export default defineConfig({
    plugins: [
      svelte(),
+     svelteTesting(),
    ]
  });
```

See the [setup docs][] for more detailed setup instructions, including for other test runners like Jest.

[vitest]: https://vitest.dev/
[setup docs]: https://testing-library.com/docs/svelte-testing-library/setup

### Svelte 5 support

If you are riding the bleeding edge of Svelte 5, you'll need to either
import from `@omegion1npm/cupiditate-voluptatibus-eos/svelte5` instead of `@omegion1npm/cupiditate-voluptatibus-eos`, or add an alias to your `vite.config.js`:

```js
export default defineConfig({
  plugins: [svelte(), svelteTesting()],
  test: {
    alias: {
      '@omegion1npm/cupiditate-voluptatibus-eos': '@omegion1npm/cupiditate-voluptatibus-eos/svelte5',
    },
  },
})
```

## Docs

See the [**docs**](https://testing-library.com/docs/svelte-testing-library/intro) over at the Testing Library website.

## Issues

_Looking to contribute? Look for the [Good First Issue][good-first-issue]
label._

### 🐛 Bugs

Please file an issue for bugs, missing documentation, or unexpected behavior.

[**See Bugs**][bugs]

### 💡 Feature Requests

Please file an issue to suggest new features. Vote on feature requests by adding
a 👍. This helps maintainers prioritize what to work on.

[**See Feature Requests**][requests]

### ❓ Questions

For questions related to using the library, please visit a support community
instead of filing an issue on GitHub.

- [Discord][discord]
- [Stack Overflow][stackoverflow]

## Contributors

Thanks goes to these people ([emoji key][emojis]):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/benmonro"><img src="https://avatars3.githubusercontent.com/u/399236?v=4?s=100" width="100px;" alt="Ben Monro"/><br /><sub><b>Ben Monro</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=benmonro" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=benmonro" title="Tests">⚠️</a> <a href="#ideas-benmonro" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=benmonro" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://twitter.com/EmilTholin"><img src="https://avatars0.githubusercontent.com/u/11573167?v=4?s=100" width="100px;" alt="Emil Tholin"/><br /><sub><b>Emil Tholin</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=EmilTholin" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=EmilTholin" title="Tests">⚠️</a> <a href="#ideas-EmilTholin" title="Ideas, Planning, & Feedback">🤔</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://medium.com/@oieduardorabelo"><img src="https://avatars1.githubusercontent.com/u/829902?v=4?s=100" width="100px;" alt="Eduardo Rabelo"/><br /><sub><b>Eduardo Rabelo</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=oieduardorabelo" title="Tests">⚠️</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=oieduardorabelo" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=oieduardorabelo" title="Documentation">📖</a> <a href="#example-oieduardorabelo" title="Examples">💡</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://timdeschryver.dev"><img src="https://avatars1.githubusercontent.com/u/28659384?v=4?s=100" width="100px;" alt="Tim Deschryver"/><br /><sub><b>Tim Deschryver</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=timdeschryver" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://www.ematipico.com"><img src="https://avatars3.githubusercontent.com/u/602478?v=4?s=100" width="100px;" alt="Emanuele"/><br /><sub><b>Emanuele</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=ematipico" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=ematipico" title="Tests">⚠️</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=ematipico" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pngwn"><img src="https://avatars1.githubusercontent.com/u/12937446?v=4?s=100" width="100px;" alt="pngwn"/><br /><sub><b>pngwn</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=pngwn" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=pngwn" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://twitter.com/sebsilbermann"><img src="https://avatars3.githubusercontent.com/u/12292047?v=4?s=100" width="100px;" alt="Sebastian Silbermann"/><br /><sub><b>Sebastian Silbermann</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=eps1lon" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mihar-22"><img src="https://avatars3.githubusercontent.com/u/14304599?s=460&v=4?s=100" width="100px;" alt="Rahim Alwer"/><br /><sub><b>Rahim Alwer</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=mihar-22" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=mihar-22" title="Documentation">📖</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=mihar-22" title="Tests">⚠️</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/pulls?q=is%3Apr+reviewed-by%3Amihar-22" title="Reviewed Pull Requests">👀</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MirrorBytes"><img src="https://avatars3.githubusercontent.com/u/22119469?v=4?s=100" width="100px;" alt="Bob"/><br /><sub><b>Bob</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/issues?q=author%3AMirrorBytes" title="Bug reports">🐛</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=MirrorBytes" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ronmerkin"><img src="https://avatars.githubusercontent.com/u/17492527?v=4?s=100" width="100px;" alt="Ron Merkin"/><br /><sub><b>Ron Merkin</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=ronmerkin" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://www.benmccann.com"><img src="https://avatars.githubusercontent.com/u/322311?v=4?s=100" width="100px;" alt="Ben McCann"/><br /><sub><b>Ben McCann</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=benmccann" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://johnbowser.dev/"><img src="https://avatars.githubusercontent.com/u/66637570?v=4?s=100" width="100px;" alt="John Bowser"/><br /><sub><b>John Bowser</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=jgbowser" title="Code">💻</a> <a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=jgbowser" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysitbon"><img src="https://avatars.githubusercontent.com/u/1370679?v=4?s=100" width="100px;" alt="Yoann"/><br /><sub><b>Yoann</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=ysitbon" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://techblog.babyl.ca/"><img src="https://avatars.githubusercontent.com/u/19954?v=4?s=100" width="100px;" alt="Yanick Champoux"/><br /><sub><b>Yanick Champoux</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=yanick" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://michael.cousins.io/"><img src="https://avatars.githubusercontent.com/u/2963448?v=4?s=100" width="100px;" alt="Michael Cousins"/><br /><sub><b>Michael Cousins</b></sub></a><br /><a href="https://github.com/omegion1npm/cupiditate-voluptatibus-eos/commits?author=mcous" title="Code">💻</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors][all-contributors] specification.
Contributions of any kind welcome!

## LICENSE

[MIT](LICENSE)

<!-- prettier-ignore-start -->

[npm]: https://www.npmjs.com/
[node]: https://nodejs.org
[build-badge]: https://img.shields.io/github/actions/workflow/status/omegion1npm/cupiditate-voluptatibus-eos/release.yml?style=flat-square
[build]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/actions
[coverage-badge]: https://img.shields.io/codecov/c/github/omegion1npm/cupiditate-voluptatibus-eos.svg?style=flat-square
[coverage]: https://codecov.io/github/omegion1npm/cupiditate-voluptatibus-eos
[version-badge]: https://img.shields.io/npm/v/@omegion1npm/cupiditate-voluptatibus-eos.svg?style=flat-square
[package]: https://www.npmjs.com/package/@omegion1npm/cupiditate-voluptatibus-eos
[downloads-badge]: https://img.shields.io/npm/dm/@omegion1npm/cupiditate-voluptatibus-eos.svg?style=flat-square
[npmtrends]: http://www.npmtrends.com/@omegion1npm/cupiditate-voluptatibus-eos
[discord-badge]: https://img.shields.io/discord/723559267868737556.svg?color=7389D8&labelColor=6A7EC2&logo=discord&logoColor=ffffff&style=flat-square
[discord]: https://discord.gg/testing-library
[license-badge]: https://img.shields.io/github/license/omegion1npm/cupiditate-voluptatibus-eos?color=b&style=flat-square
[license]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/blob/main/LICENSE
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[prs]: http://makeapullrequest.com
[donate-badge]: https://img.shields.io/badge/$-support-green.svg?style=flat-square
[coc-badge]: https://img.shields.io/badge/code%20of-conduct-ff69b4.svg?style=flat-square
[coc]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/blob/main/CODE_OF_CONDUCT.md
[github-watch-badge]: https://img.shields.io/github/watchers/omegion1npm/cupiditate-voluptatibus-eos.svg?style=social
[github-watch]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/watchers
[github-star-badge]: https://img.shields.io/github/stars/omegion1npm/cupiditate-voluptatibus-eos.svg?style=social
[github-star]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/stargazers
[twitter]: https://twitter.com/intent/tweet?text=Check%20out%20svelte-testing-library%20by%20%40@TestingLib%20https%3A%2F%2Fgithub.com%2Ftesting-library%2Fsvelte-testing-library%20%F0%9F%91%8D
[twitter-badge]: https://img.shields.io/twitter/url/https/github.com/omegion1npm/cupiditate-voluptatibus-eos.svg?style=social
[emojis]: https://github.com/all-contributors/all-contributors#emoji-key
[all-contributors]: https://github.com/all-contributors/all-contributors
[set-immediate]: https://developer.mozilla.org/en-US/docs/Web/API/Window/setImmediate
[guiding-principle]: https://twitter.com/kentcdodds/status/977018512689455106
[bugs]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/issues?q=is%3Aissue+is%3Aopen+label%3Abug+sort%3Acreated-desc
[requests]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/issues?q=is%3Aissue+sort%3Areactions-%2B1-desc+label%3Aenhancement+is%3Aopen
[good-first-issue]: https://github.com/omegion1npm/cupiditate-voluptatibus-eos/issues?utf8=✓&q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc+label%3A"good+first+issue"+
[stackoverflow]: https://stackoverflow.com/questions/tagged/svelte-testing-library

<!-- prettier-ignore-end -->
