---
layout: post
title: "Reactjs Intro and Installation"
date: 2019-08-17
tag: [reactjs]
comments: true
---

Prolog
: Reactjs is a JavaScript library for building user interfaces. Reactjs can be used for developing single page application and mobile applications. Complex React applications usually require the use of additional libraries for state management, routing, and interaction with an API. Reactjs is developed and currently maintained by <a href="https://www.facebook.com/" target="_blank">Facebook</a>.

<!--more-->

Notable Features
: - Components
: - Functional components
: - Class-based components
: - Virtual DOM
: - Lifecycle methods
: - JSX (Javascript XML)
: - Nested Elements
: - React Redux
: - React Hooks

Install Nodejs

: - For Installing Reactjs first we need to install <a href="https://nodejs.org/en/download/" target="_blank">Nodejs</a>. It will be Nice to use Node version manager tool like <a href="https://github.com/nvm-sh/nvm" target="_blank">NVM</a> to install Nodejs.

: - Get the lastest version of nodejs list from remote by using nvm command

```
nvm ls-remote
```

Select the latest stable version and install, for example

<img src="/images/node_versions.png" alt="node versions" height="200" width="200"/>

you can choose any LTS versions as like shown in the pic. for installing node

```
nvm install version
```

_nvm install 10.16.3_

then

```
nvm use version
```

Install Reactjs
: - To install Reactjs gobally

```
npm install -g create-react-app
```
