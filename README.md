# p-stream-proxy

Lightweight proxy for piping and transforming node streams between processes or over the network.

## Features

- Forward Node.js streams with minimal overhead
- Optional transform hooks for data processing
- Small, dependency-free core

## Installation

```bash
npm install p-stream-proxy
```

## Usage

Basic example (proxy a readable to a writable):

```js
const { createProxy } = require('p-stream-proxy');

// Example API — adapt to actual module exports
const proxy = createProxy({ transform: chunk => chunk });
readable.pipe(proxy).pipe(writable);
```

See the project code and tests for full examples.

## API

Exported functions:

- `createProxy(options)` — create a proxy stream. Options may include `transform` (a function) and other stream options.

(Adjust names and signatures to match the actual code in this repository.)

## Contributing

Contributions, issues, and feature requests are welcome. Please open an issue or submit a pull request.

## License

MIT

## Contact

Created by FuchsiFox — thank you for using p-stream-proxy!
