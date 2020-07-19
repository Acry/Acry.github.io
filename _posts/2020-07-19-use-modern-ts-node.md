---
title: Use modern JS in TS-Node on Arch-Linux
author: Acry
layout: post
---

## The Problem

One wants to use ES2020 or ESNEXT features with the global installed ts-node. TS-Node defaults to **ES3**.

![](/assets/images/array-flat-failing.png)

## Current versions as time of writing

- TS-Node 8.10.2
- Typescript 3.9.7
- NPM 6.14.6

## Requirements

Expecting your npm is set up like in your shell's runtime conditions:

```shell
PATH="$HOME/.node_modules/bin:$PATH"
export npm_config_prefix=~/.node_modules
```

## Installation

Install TypeScript and TS-Node globally (user-wide in `~/.node_modules`)

```shell
npm install -g ts-node
npm install -g typescript
```

Verify:

```shell
npm list -g --depth 0
├── ts-node@8.10.2
└── typescript@3.9.7
```

## Setup TypeScript properly\*

In your Terminal-Emulator:

```shell
cd ~
tsc --init
sed -i 's/"target": "ES3"/"target": "ES2020"/' tsconfig.json
```

![](/assets/images/array-flat-success.png)

\*With properly I mean good enough to use [`Array.prototype.flat()`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/flat).<br>
To set up TypeScript for your use-case see: <https://www.typescriptlang.org/docs/handbook/compiler-options.html>
