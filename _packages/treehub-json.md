---
title: Treehub.json
order: 50
---

````javascript
{
  "name": "my-example", // Required
  "version": "1.0.0", // Required. Please follow semver :)
  "components": [
    "./components.js"
  ],
  "nav": [
    "my-example-nav"
  ],
  "taskbar": [
    "my-example-taskbar"
  ],
  "page": [
    "my-example",
  ],
  "aside": [
    "my-example-aside"
  ],
  "route": "./route.js", // Will be available under POST /my-example/*
}
````
