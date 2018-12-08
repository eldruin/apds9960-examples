# Additional example programs for the [apds9960] crate [![Build Status](https://travis-ci.org/eldruin/apds9960-examples.svg?branch=master)](https://travis-ci.org/eldruin/apds9960-examples)

[apds9960]: https://crates.io/crates/apds9960

This repository contains additional example programs using the APDS9960 I2C
temperature sensor with an STM32F3Discovery board.

These examples expect that you connect the APDS9960 device to the pins PB6 (SCL)
and PB7 (SDA) of the discovery board.

For example, to run the f3-proximity-display example:
First, connect your discovery board per USB, then connect OpenOCD in a terminal with:
```
openocd -f interface/stlink-v2-1.cfg -f target/stm32f3x.cfg
```

Then on another terminal run:
```
git clone https://github.com/eldruin/apds9960-examples
cd apds9960-examples
cargo run --example f3-proximity-display
```

## License

Licensed under either of

 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT) at your option.

### Contributing

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.

