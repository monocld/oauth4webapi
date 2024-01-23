# Interface: ValidateJWTAccessTokenOptions

[💗 Help the project](https://github.com/sponsors/panva)

## Table of contents

### Experimental

- [[experimental\_customFetch]](ValidateJWTAccessTokenOptions.md#experimental_customfetch)

### Properties

- [[clockSkew]](ValidateJWTAccessTokenOptions.md#clockskew)
- [[clockTolerance]](ValidateJWTAccessTokenOptions.md#clocktolerance)
- [headers](ValidateJWTAccessTokenOptions.md#headers)
- [requireDPoP](ValidateJWTAccessTokenOptions.md#requiredpop)
- [signal](ValidateJWTAccessTokenOptions.md#signal)

## Experimental

### [experimental\_customFetch]

• `Optional` **[experimental\_customFetch]**: (`input`: `RequestInfo` \| [`URL`]( https://developer.mozilla.org/docs/Web/API/URL ), `init?`: `RequestInit`) => [`Promise`]( https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Promise )\<[`Response`]( https://developer.mozilla.org/docs/Web/API/Response )\>

This is an experimental feature, it is not subject to semantic versioning rules. Non-backward
compatible changes or removal may occur in any future release.

See [experimental_customFetch](../variables/experimental_customFetch.md) for its documentation.

## Properties

### [clockSkew]

• `Optional` **[clockSkew]**: `number`

Same functionality as in [Client](Client.md)

___

### [clockTolerance]

• `Optional` **[clockTolerance]**: `number`

Same functionality as in [Client](Client.md)

___

### headers

• `Optional` **headers**: [`Record`]( https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type )\<`string`, `string`\> \| [`string`, `string`][] \| [`Headers`]( https://developer.mozilla.org/docs/Web/API/Headers )

Headers to additionally send with the HTTP Request(s) triggered by this function's invocation.

___

### requireDPoP

• `Optional` **requireDPoP**: `boolean`

Indicates whether DPoP use is required.

___

### signal

• `Optional` **signal**: [`AbortSignal`]( https://developer.mozilla.org/docs/Web/API/AbortSignal ) \| () => [`AbortSignal`]( https://developer.mozilla.org/docs/Web/API/AbortSignal )

An AbortSignal instance, or a factory returning one, to abort the HTTP Request(s) triggered by
this function's invocation.

**`Example`**

A 5000ms timeout AbortSignal for every request

```js
const signal = () => AbortSignal.timeout(5_000) // Note: AbortSignal.timeout may not yet be available in all runtimes.
```

## Hierarchy

- [`HttpRequestOptions`](HttpRequestOptions.md)

  ↳ **`ValidateJWTAccessTokenOptions`**