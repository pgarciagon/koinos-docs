# Serializer class

`Serializer` encodes and decodes Protocol Buffer messages from a descriptor.

<!-- example: reference-koilib-serializer -->
```javascript
--8<-- "examples/javascript/references/koilib-api-tour/index.js:serializer"
```

[View complete file](https://github.com/pgarciagon/koinos-docs/blob/main/examples/javascript/references/koilib-api-tour/index.js) ·
[Run example](https://stackblitz.com/fork/github/pgarciagon/koinos-docs/tree/main/examples/javascript/references/koilib-api-tour)

This local round trip needs no network connection and checks that the decoded
message matches the input.
