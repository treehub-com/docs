---
title: Routes
order: 100
---

# Routes

Routes are a way to perform off-thread tasks or tasks that need to persist data.

### Route initialization

````javascript
module.exports = async ({
  LevelUpBackend, // LevelUp compatible backend class
  pathPrefix, // Prefix to use for any instantiated LevelUp databases
}) => {
  // Perform initialization
  ...

  // Return route function
  return routeFunction;
}
````

### Route execution

````javascript
async function routeFunction({
  route, // The full route minus the prefix (called: /my-package/foo/bar => route: /foo/bar)
  body, // The JSON object
}) {
  // Perform route execution
  ...

  // Thrown errors will result in a 500 with the body sent to {message: error.message}
  // To set a status code set error.code = xxx

  // Result will be json encoded/stringified
  return result;
}
````
