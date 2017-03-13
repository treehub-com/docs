---
title: Startup
order: 20
---

# Startup

1. Ensure required packages are installed
    - `api`
    - `app`
    - `package-manager`
    - `what`
1. Start Server
    1. Register core (`_`) routes
    1. Loop through packages and register routes
1. Get `/packages.json` and save to `window.packages`
1. For each package:
    1. Add a script tag to head for each component
1. Write `<th-app>` to body
