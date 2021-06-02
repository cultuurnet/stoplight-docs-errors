# URL

This page contains an overview of all possible error types inside the `https://api.publiq.be/probs/url/` namespace that can be returned by publiq's APIs.

> APIs can also use their own types for errors. The types below are used in situations where an API has no more specific type for an error related to a the requested URL.

## not-found

-   **Type:** `https://api.publiq.be/probs/url/not-found`
-   **Title**: `URL not found`
-   **Status**: `404`

The URL you requested is not available. Possible causes include:

-   The endpoint does not exist
-   An id or slug of a resource in the path does not exist or is invalid

## method-not-supported

-   **Type:** `https://api.publiq.be/probs/url/method-not-supported`
-   **Title**: `Method not supported`
-   **Status**: `400`

The URL you requested exists, but the method you are trying to use is not supported. For example the endpoint may support `GET`, but not `PUT`.

## query-parameter-missing

-   **Type:** `https://api.publiq.be/probs/url/query-parameter-missing`
-   **Title**: `Query parameter missing`
-   **Status**: `400`

A required query parameter is missing. More info on what parameter specifically can be found in the `detail` property of the response.

## query-parameter-invalid

-   **Type:** `https://api.publiq.be/probs/url/query-parameter-invalid`
-   **Title**: `Query parameter invalid`
-   **Status**: `400`

The value of a given query parameter is invalid. More info on what parameter specifically can be found in the `detail` property of the response.

Also used when a query parameter references another resource and that resource is not found.

In some cases, depending on the API, this can also be returned when an invalid parameter name is used.
