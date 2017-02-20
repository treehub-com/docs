---
title: Startup
order: 20
---

# Startup

1. Start Server
    1. Register core (`_`) routes
    1. Loop through packages and register routes
1. If required packages are not installed:
    1. Install required packages
    1. Start again at #1
1. Get `/packages.json` and save to `window.packages`
1. For each package:
    1. Add a script tag to head for each component
1. Write `<th-app>` to body
