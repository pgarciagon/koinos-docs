# Utility functions

Koilib exports helpers for units, encodings, hashes, addresses, and bundled
standard ABIs.

<!-- example: reference-koilib-utils -->
```javascript
--8<-- "examples/javascript/references/koilib-api-tour/index.js:utils"
```

[View complete file](https://github.com/pgarciagon/koinos-docs/blob/main/examples/javascript/references/koilib-api-tour/index.js) ·
[Run example](https://stackblitz.com/fork/github/pgarciagon/koinos-docs/tree/main/examples/javascript/references/koilib-api-tour)

`formatUnits` converts an integer amount in the token's smallest unit into a
human-readable decimal string without changing blockchain state.
