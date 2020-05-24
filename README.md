# textventure/stories

[Textventure](https://textventure.github.io/) [stories](STORIES.md).

See [STORIES.md](STORIES.md).

## Prerequisites

- [Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)

## Installation

Clone repository:

```sh
$ git clone https://github.com/textventure/stories.git
$ cd stories
```

Install dependencies:

```sh
$ npm install
```

## Scripts

### `npm run clean`

Removes `build` directory.

### `npm run copy`

Copies YAML files in `src` to `build` directory.

### `npm run copy`

Copies `src` files to `build` directory following a flat directory structure (only files, no subdirectories).

### `npm run deploy`

Deploys `build` to `gh-pages` with [gitploy](https://www.npmjs.com/package/gitploy).

### `npm run lint`

Checks file formatting with [prettier](https://prettier.io/docs/en/cli.html#--check).

### `npm run lint:fix`

Formats the files with [prettier](https://prettier.io/docs/en/cli.html#--write).
