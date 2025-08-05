# Caching

## Request Memoization

- While rendering a route, the first time a particular request is called, its result will not be in memory and it'll be a cache MISS.
Therefore, the function will be executed, and the data will be fetched from the external source, and the result will be stored in memory.
Subsequent function calls of the request in the same render pass will be a cache HIT, and the data will be returned from memory without executing the function.
Once the route has been rendered and the rendering pass is complete, memory is "reset" and all request memoization entries are cleared.
- Memoization only applies to the GET method in fetch requests.
- For cases where fetch is not suitable (e.g. some database clients, CMS clients, or GraphQL clients), you can use the React cache function to memoize functions.
- It doesn't apply to fetch requests in Route Handlers as they are not a part of the React component tree.
- The cache lasts the lifetime of a server request until the React component tree has finished rendering.

----

# Data Cache
- In the browser, the cache option of fetch indicates how a request will interact with the browser's HTTP cache, in Next.js, the cache option indicates how a server-side request will interact with the server's Data Cache.
- In development mode, fetch data is reused for Hot Module Replacement (HMR), and caching options are ignored for hard refreshes.
