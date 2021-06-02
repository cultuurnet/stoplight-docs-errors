# Body

This page contains an overview of all possible error types inside the `https://api.publiq.be/probs/body/` namespace that can be returned by publiq's APIs.

> APIs can also use their own types for errors. The errors below are used in general situations when an API has no specific type for an error related to a the body included in a request.

## missing

-   **Type:** `https://api.publiq.be/probs/body/missing`
-   **Title**: `Body missing`
-   **Status**: `400`

The endpoint requires a body inside the request but none was included.

## invalid-syntax

-   **Type:** `https://api.publiq.be/probs/body/invalid-syntax`
-   **Title**: `Invalid body syntax`
-   **Status**: `400`

The body you included (typically JSON) has an invalid syntax and cannot be parsed by the API.

## invalid-data

-   **Type:** `https://api.publiq.be/probs/body/invalid-data`
-   **Title**: `Invalid body data`
-   **Status**: `400`

The body you included (typically JSON) has invalid or missing properties. The problem detail should contain more info about what property specifically, and in some cases a [jsonPointer](./http-body.md#jsonPointer) may be included.