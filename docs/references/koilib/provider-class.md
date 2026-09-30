# Provider class

`Provider` connects Koilib to a Koinos JSON-RPC endpoint. Read calls such as
`getHeadInfo()` do not require an account or mana.

<!-- example: reference-koilib-provider -->
```javascript
--8<-- "examples/javascript/references/koilib-api-tour/index.js:provider"
```

[View complete file](https://github.com/pgarciagon/koinos-docs/blob/main/examples/javascript/references/koilib-api-tour/index.js) ·
[Run example](https://stackblitz.com/fork/github/pgarciagon/koinos-docs/tree/main/examples/javascript/references/koilib-api-tour)

The complete example reads the current mainnet height.
