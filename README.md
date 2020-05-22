[![Jovo Framework](../docs/img/jovo-header.png)](https://www.jovo.tech)

<p align="center">The development framework for cross-platform voice apps</p>

<p align="center">
<a href="https://www.jovo.tech/docs/"><strong>Documentation</strong></a> -
<a href="https://github.com/jovotech/jovo-cli"><strong>CLI </strong></a> -
<a href="https://github.com/jovotech/jovo-sample-voice-app-nodejs"><strong>Sample App </strong></a> - <a href="https://github.com/jovotech/jovo-framework/tree/master/.github/CONTRIBUTING.md"><strong>Contributing</strong></a> - <a href="https://twitter.com/jovotech"><strong>Twitter</strong></a></p>
<br/>

<p align="center">
<a href="https://travis-ci.org/jovotech/jovo-framework" target="_blank"><img src="https://travis-ci.org/jovotech/jovo-framework.svg?branch=master"></a>
<a href="https://www.npmjs.com/package/jovo-framework" target="_blank"><img src="https://badge.fury.io/js/jovo-framework.svg"></a>
<a href="./CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a>
<a href="https://slackin-uwinbxqkfx.now.sh" target="_blank"><img src="https://slackin-uwinbxqkfx.now.sh/badge.svg"></a>
<a href="https://twitter.com/intent/tweet?text=🔈 Build cross-platform voice apps for Alexa and Google Assistant with @jovotech https://github.com/jovotech/jovo-framework/" target="_blank"><img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
</p>
<br/>

# Jovo PulseLabs Plugin

Install package:

```sh
npm install jovo-plugin-pulselabs --save
```

Add the plugin to your `app.js` file:

```js
// src/app.js

const { PulseLabs } = require ('jovo-plugin-pulselabs');

app.use( new PulseLabs({ apiKey: 'yourApiKey' }) );
```

# Configuring additional options

You can pass additional configuration options as below:

```js

app.use( new PulseLabs({ apiKey: 'yourApiKey' , options: { timeout: 2000, debug: true } }) );
```

***debug*** - ```boolean``` logs helpful debugging information
<br/>
***timeout*** - ```number``` timeouts requests after given milliseconds
