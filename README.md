# detect-pi

Detect if node is currently running on a raspberry pi.

## Usage

`npm install detect-rpi --save`

```js
const isPi = require('detect-rpi');

if (isPi()) {
  console.log('Running on Raspberry Pi!');
} else {
  // ...
}
```

## How?

Reads /proc/cpuinfo and checks if 'Hardware' === 'BCM2709'.
