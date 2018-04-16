# QWER Music Box

## Introduction

QWER Music Box is a music player built under electron, supports Windows, Linux and OS X.

It is aiming to make a (R)eborn of three popular music players in China.

+ Q(Q) Music
+ Ku(W)o Music
+ Net(E)ase Cloud Music

Other music players would be supported in the future.

+ KuGou Music
+ XiaMi Music

Almost all of the players listed above (except NetEase Cloud Music) doesn't provide a client on Linux.
That's why this project is started.

## Releases

## Development

### Install

* **Note: requires a node version >= 7 and an npm version >= 4.**

```bash
$ git clone https://github.com/tc-imba/qwer-music-box
$ cd qwer-music-box
$ yarn
```

### Run

Start the app in the `dev` environment. This starts the renderer process in [**hot-module-replacement**](https://webpack.js.org/guides/hmr-react/) mode and starts a webpack dev server that sends hot updates to the renderer process:

```bash
$ npm run dev
```

Alternatively, you can run the renderer and main processes separately. This way, you can restart one process without waiting for the other. Run these two commands **simultaneously** in different console tabs:

```bash
$ npm run start-renderer-dev
$ npm run start-main-dev
```

### Packaging

To package apps for the local platform:

```bash
$ npm run package
```

To package apps for all platforms:

First, refer to [Multi Platform Build](https://www.electron.build/multi-platform-build) for dependencies.

Then,
```bash
$ npm run package-all
```

To package apps with options:

```bash
$ npm run package -- --[option]
```

To run End-to-End Test

```bash
$ npm run build
$ npm run test-e2e
```

:bulb: You can debug your production build with devtools by simply setting the `DEBUG_PROD` env variable:
```bash
DEBUG_PROD=true npm run package
```

## Reference

+ [electron-react-boilerplate](https://github.com/chentsulin/electron-react-boilerplate)
+ [MusicBox](https://github.com/HuberTRoy/MusicBox)
+ [NetEase-MusicBox](https://github.com/bluetomlee/NetEase-MusicBox)

## License

MIT
