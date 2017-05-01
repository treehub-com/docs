---
title: treehub.json
order: 50
---
# treehub.json

````javascript
{
  "name": "my-example", // Required
  "description": "An example package", // Required
  "components": [ // Components to fetch on load. These will be executed before the app is initialized, so don't do work in them
    "./components.js"
  ],
  "files": [ // Additional files you want included
    "./image.png"
  ],
  "route": "./route.js", // Will be available under POST /my-example/*
  "provides": { // Tells other packages what you provide
    "app": { // Provide app level things
      "nav": [
        "my-example-nav"
      ],
      "taskbar": [
        "my-example-taskbar"
      ],
      "page": "my-example",
      "aside": "my-example-aside"
    }
  }
}
````
