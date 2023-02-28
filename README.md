# semantic-release-pulsar-config

[**semantic-release**](https://github.com/semantic-release/semantic-release) shareable config to publish [Pulsar](https://www.pulsar-edit.dev) packages.

[![Build Status](https://github.com/ewanharris/semantic-release-pulsar-config/workflows/Test/badge.svg)](https://github.com/ewanharris/semantic-release-pulsar-config/actions?query=workflow%3ATest+branch%3Amaster) [![npm latest version](https://img.shields.io/npm/v/semantic-release-pulsar-config/latest.svg)](https://www.npmjs.com/package/semantic-release-pulsar-config)


## Plugins

This shareable configuration use the following plugins:

- [`@semantic-release/commit-analyzer`](https://github.com/semantic-release/commit-analyzer)
- [`@semantic-release/release-notes-generator`](https://github.com/semantic-release/release-notes-generator)
- [`@semantic-release/github`](https://github.com/semantic-release/github)
- [`@semantic-release/changelog`](https://github.com/semantic-release/changelog)
- [`semantic-release-pulsar`](https://github.com/ewanharris/semantic-release-pulsar)
- [`@semantic-release/git`](https://github.com/semantic-release/git)

## Install

```bash
$ npm install --save-dev semantic-release semantic-release-pulsar-config
```

## Usage

The shareable config can be configured in the [**semantic-release** configuration file](https://github.com/semantic-release/semantic-release/blob/master/docs/usage/configuration.md#configuration):

```json
{
  "extends": "semantic-release-pulsar-config"
}
```

## Configuration

See each [plugin](#plugins) documentation for required installation and configuration steps.

### Overwritten options

This following options are set by this shareable config:

| Option                                                       | Value                                             |
| ------------------------------------------------------------ | ------------------------------------------------- |
| [`message`](https://github.com/semantic-release/git#message) | chore(release): \${nextRelease.version} [skip ci] |

Other options use their default values. See each [plugin](#plugins) documentation for available options.

## Credits

This package is a fork of the original [apm-config](https://github.com/semantic-release/apm-config) package.