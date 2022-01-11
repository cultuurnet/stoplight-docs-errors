# Header

This page contains an overview of all possible error types inside the `https://api.publiq.be/probs/header/` namespace that can be returned by publiq's APIs.

> APIs can also use their own types for errors. The types below are used in situations where an API has no specific type for an error related to a header.

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

## not-acceptable

-   **Type:** `https://api.publiq.be/probs/header/not-acceptable`
-   **Title**: `Not Acceptable`
-   **Status**: `406`

This error is returned if the request to the API included an `Accept` header with a content-type that the API does not support, and the API is unwilling or unable to return a default content-type instead.

For example, you might be doing a request with `Accept: application/xml` while the API does not support XML and does not want to return a default format like JSON instead. In this case the API will return this error.

To fix this error, do not use an `Accept` header in your requests or set it to a content-type that the API supports (most often `application/json` and/or `application/json+ld`).

For more info, see https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/406
