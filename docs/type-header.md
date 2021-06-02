# Header

This page contains an overview of all possible error types inside the `https://api.publiq.be/probs/header/` namespace that can be returned by publiq's APIs.

> APIs can also use their own types for errors. The types below are used in situations where an API has no more specific type for an error related to a header.

## missing

-   **Type:** `https://api.publiq.be/probs/header/missing`
-   **Title**: `Header missing`
-   **Status**: `400`

A required header is missing. More info on what header specifically can be found in the `detail` property of the response.

## invalid

-   **Type:** `https://api.publiq.be/probs/header/invalid`
-   **Title**: `Header invalid`
-   **Status**: `400`

The value of a given header is invalid. More info on what header specifically can be found in the `detail` property of the response.
