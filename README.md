# joi-enum-extensions

Joi extensions for enum mapping.

[![Build Status](https://travis-ci.org/logoran/joi-enum-extensions.svg?branch=master)](https://travis-ci.org/logoran/joi-enum-extensions)
[![NSP Status](https://nodesecurity.io/orgs/logoran/projects/be6a2f14-db5f-48f1-a9ab-8f74207670e1/badge)](https://nodesecurity.io/orgs/logoran/projects/be6a2f14-db5f-48f1-a9ab-8f74207670e1)
[![Known Vulnerabilities](https://snyk.io/test/github/logoran/joi-enum-extensions/badge.svg)](https://snyk.io/test/github/logoran/joi-enum-extensions)

Lead Maintainer: [Leo Long](https://github.com/yujunlong2000)

# Usage

The `.map` method can be chained onto the base Joi number schema:

```js
const BaseJoi = require('joi');
const Enum = require('joi-enum-extensions');
const Joi = BaseJoi.extend(Enum);

const schema = Joi.number().map({
    admin : 1,
    vendor: 2,
    client: 3
});
```

# API
See the [API Reference](https://github.com/logoran/joi-enum-extensions/blob/master/API.md).