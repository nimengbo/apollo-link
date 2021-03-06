# Change log

### vNEXT

### 1.5.3
- updated dependency on `apolloLink.httpCommon` [#522](https://github.com/apollographql/apollo-link/pull/522)

### 1.5.2
- fix issue where execution result with only `errors` key fired the `next` event
- Add missing rollup alias and make http-common exported as `apolloLink.httpCommon` [#522](https://github.com/apollographql/apollo-link/pull/522)

### 1.5.1
- update apollo link with zen-observable-ts [PR#515](https://github.com/apollographql/apollo-link/pull/515)

### 1.5.0
- New useGETForQueries option: if set, uses GET for queries (but not mutations)

### 1.4.0
- move logic to apollo-link-http-core [PR#364](https://github.com/apollographql/apollo-link/pull/364)
- follow the spec properly for GET requests [PR#490](https://github.com/apollographql/apollo-link/pull/490)
- ApolloLink upgrade

### 1.3.3
- ApolloLink upgrade
- Allow graphql results to fire even if there is a network error

### 1.3.2
- Update to graphql@0.12

### 1.3.1
- export options as named interface [TypeScript]
- Fix typescript bug with destructuring of parameter in createHttpLink ([#189](https://github.com/apollographql/apollo-link/issues/189))

### 1.3.0
- changed to initially parsing response as text to improve error handling
- cleaned up error handling types and added docs
- changed peer-dependency of apollo-link to actual dependency

### 1.2.0
- moved to better rollup build
- support for persisted queries by opting out of sending the query

### v1.1.0
- support dynamic endpoints using `uri` on the context
- the request not attaches the raw response as `response` on the context. This can be used to access response headers or more

### v1.0.0
- official release, not changes

### v0.9.0
- changed `fetcherOptions` to be `fetchOptions` and added a test for using 'GET' requests

### v0.8.0
- throw error on empty ExectionResult (missing)
- support setting credentials, headers, and fetcherOptions in the setup of the link
- removed sending of context to the server and allowed opt-in of sending extensions
