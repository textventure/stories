# textventure/stories

[![Build Status](https://travis-ci.org/textventure/stories.svg?branch=master)](https://travis-ci.org/textventure/stories)

[Play](https://textventure.github.io/play/) [textventure](https://textventure.github.io/) [stories](STORIES.md).

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

### `npm start`

Starts a static file server with [http-server](https://www.npmjs.com/package/http-server). Use with [ngrok](https://ngrok.com/) to test stories.

## Testing

To test a story, you have 2 options:

1. Upload your story to a [Gist](https://gist.github.com/)
2. Or start a local server with tunnelling

### Upload to Gist

1. Create a new [Gist](https://gist.github.com/).
2. Once the gist is created, click on the <kbd>Raw</kbd> button and copy the URL.
3. Load the URL in [textventure/play](https://textventure.github.io/play/).
4. Reload the page after an edit.

### Tunnel local server

1. Start local server:
   ```sh
   $ npm start
   ```
2. Expose local server with [ngrok](https://ngrok.com/):
   ```sh
   $ ngrok http 8080
   ```
3. Open the secure public URL created by ngrok:
   ```sh
   $ open https://abc123.ngrok.io # replace `abc123`
   ```
4. Search through the directory listing to find your story and copy the URL.
5. Load the URL in [textventure/play](https://textventure.github.io/play/).
6. Hard reload the page after an edit.
