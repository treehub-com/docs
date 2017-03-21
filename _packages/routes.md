---
title: Routes
order: 100
---

# Routes

Routes are a way to perform off-thread tasks or tasks that need to persist data.

### Route initialization

````javascript
module.exports = ({
  LevelUpBackend, // LevelUp compatible backend class
  pathPrefix, // Prefix to use for any instantiated LevelUp databases
}) => {
  // Perform synchronous initialization
  ...

  // Return route function
  return routeFunction;
}
````

### Route execution

````javascript
const routeFunction = async ({
  route, // The full route minus the prefix (called: /my-package/foo/bar => route: /foo/bar)
  body, // The JSON object
}) => {

}
````
