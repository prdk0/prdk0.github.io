---
layout: post
title: "Reactjs Proxy configuration"
date: 2019-11-17
tag: [reactjs]
comments: true
---

A Single line of Reactjs proxy can be configured in package.json file inside react app but more than one Reactjs proxy is configured with the help of a middleware called [http proxy middleware](https://github.com/chimurai/http-proxy-middleware "proxy middleware"){:target="\_blank"}.

<!--more-->

### Configure Proxy Api

First we need to install [http proxy middleware](https://github.com/chimurai/http-proxy-middleware "proxy middleware"){:target="\_blank"} as a project dependency.

```bash
npm install --save-dev http-proxy-middleware
```

create a file `setupProxy.js`, you have to create exactly the same name for the file inside your src directory in your reactjs project.

```javascript
const proxy = require("http-proxy-middleware");
module.exports = function(app) {
  app.use(
    "/your-api",
    proxy({
      target: "api-domain"
    })
  );
};
```

In this code first you need to import the library `http-proxy-middleware`. Then export the the proxy configuration using `module.exports`. `"your-api"` is the relative path of your api and `"your domain"` is the domain of your api.

you need to maintain `commonjs` syntax inside the `setupProxy.js` you cannot use `es6` syntax. The `setupProxy.js` will automatically load when the app gets loaded.
