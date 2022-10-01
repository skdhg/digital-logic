# Digital Logic

A collection of digital logic utilities

# Installation

```sh
$ npm install digital-logic
```

# Included Utilities
* ✅ Logic gates
* ✅ Half adder
* ✅ Full adder
* ✅ Half subtractor
* ✅ Full subtractor
* ✅ Logic gates - truth table generator
* ✅ Signal generator
* ✅ Bits utilities *partial*
* ✅ Number system utilities *partial*

# TODO
* Multiplexer
* Demultiplexer
* Encoder
* Decoder
* K-Map Utilities
* and more...

# Examples

## Logic Gates

```js
const { LogicGates } = require("digital-logic");

LogicGates.AND(0, 0); // 0
LogicGates.AND(0, 1); // 0
LogicGates.AND(1, 0); // 0
LogicGates.AND(1, 1); // 1
```

## Full Adder

```js
const { Adder } = require("digital-logic");

const values = {
    input1: 1,
    input2: 1,
    carry: 1
};

Adder.fullAdder(input1, input2, carry); // { sum: 1, carry: 1 }
```

## Generate 3-bit signals

```js
const { BitsUtil } = require("digital-logic");

BitsUtil.generateSignals(3);
/*
[
    [0, 0, 0],
    [0, 0, 1],
    [0, 1, 0],
    [0, 1, 1],
    [1, 0, 0],
    [1, 0, 1],
    [1, 1, 0],
    [1, 1, 1]
]
*/
```