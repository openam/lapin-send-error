# Lapin Send Error
[![Version npm](https://img.shields.io/npm/v/@sinet/lapin-send-error.svg?style=flat)](https://www.npmjs.com/package/@sinet/lapin-send-error)
[![Build Status][ci-badge]][ci-badge-link]
[![Dependency Status][david-badge]][david-badge-link]
[![devDependency Status][david-dev-badge]][david-dev-badge-link]

Error handling for [Lapin](https://github.com/sinet/lapin) calls. Handles fail returns without nesting, concatenates error codes.

## Usage

```bash
npm install @sinet/lapin-send-error --save
```

### Example
If you receive an error from a database query or remote lapin call easily handle it with:

```javascript
const sendError = require( '@sinet/lapin-send-error' );

if ( error ) {
	return sendError( send, error, 'code' );
}
```

The first parameter is the `send` object from Lapin.

## Contributing
All pull requests must follow [coding conventions and standards](https://github.com/sinet/coding-conventions).

[david-badge]: https://david-dm.org/sinet/lapin-send-error.svg
[david-badge-link]: https://david-dm.org/sinet/lapin-send-error
[david-dev-badge]: https://david-dm.org/sinet/lapin-send-error/dev-status.svg
[david-dev-badge-link]: https://david-dm.org/sinet/lapin-send-error
[david-dev-badge-link]: https://david-dm.org/sinet/lapin-send-error#info=devDependencies
[ci-badge]: https://circleci.com/gh/sinet/lapin-send-error.svg?style=shield
[ci-badge-link]: https://circleci.com/gh/sinet/lapin-send-error
