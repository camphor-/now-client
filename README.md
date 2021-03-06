# now-client-camera

[![Build Status](https://travis-ci.org/camphor-/now-client-camera.svg?branch=master)](https://travis-ci.org/camphor-/now-client-camera)
[![Dependency Status](https://david-dm.org/camphor-/now-client-camera.svg)](https://david-dm.org/camphor-/now-client-camera)
[![devDependency Status](https://david-dm.org/camphor-/now-client-camera/dev-status.svg)](https://david-dm.org/camphor-/now-client-camera#info=devDependencies)

## Requirements
- Node.js v8+

## Instruction for users
- Install: `npm install -g now-client-camera`
- Run: `now-client-camera`

## Instruction for developers
- Install: `npm install`
- Run: `./bin/now-client-camera.js`

## Options
- `now-client-camera --driver=raspistill http://192.168.1.128:3000`
- `DEBUG=now-client-camera now-client-camera --driver=sample http://192.168.1.128:3000`
- `now-client-camera --driver=sample --authorization='Basic <token>' http://192.168.1.128:3000`

### Drivers
Specify a driver with `--driver=` option. (default: `sample`)

#### raspistill
Raspberry Pi Camera Module

Environment variables:
- `RASPISTILL_WIDTH` - Width of a picture (default: 320)
- `RASPISTILL_HEIGHT` - Height of a picture (default: 240)

#### imagesnap
MacBook

Note: Install [imagesnap](https://github.com/rharder/imagesnap) for using this driver.

#### sample
Sample JPEG image
