# Deepgram Voicebot 

A demo that shows how to use the [Deepgram Speech-to-Speech API]() to build a voicebot.

- [Prerequisites](#prerequisites)
- [Getting started](#getting-started)

## Prerequisites

- [Node v20](https://nodejs.org/en/download/) or higher (though I recommend installing it through [nvm](https://github.com/nvm-sh/nvm#installing-and-updating))
- Optional: [yarn](https://classic.yarnpkg.com/en/docs/install)

## Getting started 

Assuming you want to develop "locally", i.e. bring-your-own-key, just set a `DEEPGRAM_API_KEY`
environment variable and run the `dev` command. Any DG key will do, it just needs `usage:write`.

**Remember:** use minimally-privileged keys, avoid sending them in shell commands, and avoid saving
them as plaintext to files! One secure approach is to use a CLI-compatible password manager like
[pass](https://www.passwordstore.org/) or [bitwarden](https://bitwarden.com/help/cli/). A `pass`
example:

```sh
DEEPGRAM_API_KEY=$(pass deepgram/my-key) yarn dev
```

When Next.js starts up, it'll give you a localhost URL to visit.
