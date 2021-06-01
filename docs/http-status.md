# Status codes

Every error response uses a HTTP status code within the 400 or 500 range.

The most common status codes are:

*   `400` **Bad request**: A query parameter, part of the response body, or other part of the request (not covered by other statuses) is malformed, invalid or unrecognized.
*   `401` **Unauthorized**: The request is missing the required authentication info, or the credentials that are used are invalid or expired. (See the [Authentication docs](https://publiq.stoplight.io/docs/authentication/docs/errors.md#unauthorized) for more info)
*   `403` **Forbidden**: The request is successfully authenticated, but you do not have permission to perform it on the given API or resource with the used credentials. (See the [Authentication docs](https://publiq.stoplight.io/docs/authentication/docs/errors.md#forbidden) for more info)
*   `404` **Not found**: The requested URL does not exist. Can either be because the endpoint does not exist, or a resource id or slug used in the path does not exist.
