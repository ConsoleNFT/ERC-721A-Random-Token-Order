# ERC-721A-Random-Token-Order

This sample contract shows ERC-721A with random token order used for JSONs. Tokens still start from 0, but their JSON representation in TokenURI function goes randomly.

This is not a true VRF, it is a simple implementation omitting getting the random number from third party source.


## Features

- Easy to work with
- Cheap mint costs (kind of)

## Downsides

- Compared to pure ERC-721A mint costs 200k gas because of Simple VRF / Token randomizer, where in ERC-721A mint is ~70k gas
- However in multiple mints in one tx gas costs goes down
- I guess this can be further improved
