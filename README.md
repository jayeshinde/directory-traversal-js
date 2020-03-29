# Directory Traversal JS


> Safely upload files and concat paths

Directory traversal (also known as file path traversal) is a web security vulnerability that allows an attacker to read arbitrary files on the server

## Install

```sh
$ npm install --save directory-traversal-js
```

## Usage
```js
var directoryTraversalManager = require('directory-traversal-js');

const path = directoryTraversalManager.safeJoin(rootPath, filename)
```

```ts
import { safeJoin } from 'directory-traversal-js';

const path: string = safeJoin(rootPath, filename);
```

## Explanation

safeJoin throws an error in case a directory traversal has been detected or return the joined path if not.
