# api documentation for  [agenda-ui (v0.0.7)](https://github.com/moudy/agenda-ui)  [![npm package](https://img.shields.io/npm/v/npmdoc-agenda-ui.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-agenda-ui) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-agenda-ui.svg)](https://travis-ci.org/npmdoc/node-npmdoc-agenda-ui)
#### UI for Agenda

[![NPM](https://nodei.co/npm/agenda-ui.png?downloads=true)](https://www.npmjs.com/package/agenda-ui)

[![apidoc](https://npmdoc.github.io/node-npmdoc-agenda-ui/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-agenda-ui_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-agenda-ui/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-agenda-ui/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-agenda-ui/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Moudy"
    },
    "bugs": {
        "url": "https://github.com/moudy/agenda-ui/issues"
    },
    "dependencies": {
        "ejs": "^1.0.0",
        "express": "^4.3.2",
        "rsvp": "^3.0.9",
        "speakingurl": "^0.9.1"
    },
    "description": "UI for Agenda",
    "devDependencies": {
        "agenda": "^0.6.12",
        "broccoli": "^0.12.1",
        "broccoli-browserify": "^0.1.0",
        "broccoli-clean-css": "^0.1.5",
        "broccoli-cli": "0.0.1",
        "broccoli-merge-trees": "^0.1.3",
        "broccoli-middleware": "0.0.1",
        "broccoli-sass": "^0.1.4",
        "broccoli-template-builder": "0.0.4",
        "broccoli-uglify-js": "^0.1.3",
        "countdown": "^2.3.0",
        "ember-cli": "0.0.39",
        "ember-template-compiler": "^1.6.0-beta.5",
        "handlebars": "^1.1.0",
        "highlight.js": "^8.0.0",
        "jquery": "^2.1.1",
        "lodash": "^2.4.1",
        "moment": "^2.6.0",
        "moment-countdown": "0.0.1",
        "moment-duration-format": "^1.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "c7d1dc4898220539caa53b19ced011a07d13ecf7",
        "tarball": "https://registry.npmjs.org/agenda-ui/-/agenda-ui-0.0.7.tgz"
    },
    "gitHead": "3175d4d6a900318634d9797e834ddd8bc40d80c3",
    "homepage": "https://github.com/moudy/agenda-ui",
    "keywords": [
        "agenda"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "moudy",
            "email": "moudy.elkammash@gmail.com"
        }
    ],
    "name": "agenda-ui",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/moudy/agenda-ui.git"
    },
    "scripts": {
        "dev": "nodemon --ignore tmp/ --ignore app/ --ignore node_modules/ dev.js",
        "prepublish": "./scripts/build",
        "test": "mocha"
    },
    "version": "0.0.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module agenda-ui](#apidoc.module.agenda-ui)
1.  [function <span class="apidocSignatureSpan">agenda-ui.</span>store (agenda)](#apidoc.element.agenda-ui.store)
1.  object <span class="apidocSignatureSpan">agenda-ui.</span>store.prototype

#### [module agenda-ui.store](#apidoc.module.agenda-ui.store)
1.  [function <span class="apidocSignatureSpan">agenda-ui.</span>store (agenda)](#apidoc.element.agenda-ui.store.store)

#### [module agenda-ui.store.prototype](#apidoc.module.agenda-ui.store.prototype)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>buildQuery (queryParams)](#apidoc.element.agenda-ui.store.prototype.buildQuery)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>count (options)](#apidoc.element.agenda-ui.store.prototype.count)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>data (query)](#apidoc.element.agenda-ui.store.prototype.data)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>definitionObjects ()](#apidoc.element.agenda-ui.store.prototype.definitionObjects)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>definitions (query)](#apidoc.element.agenda-ui.store.prototype.definitions)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>jobs (query)](#apidoc.element.agenda-ui.store.prototype.jobs)
1.  [function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>meta ()](#apidoc.element.agenda-ui.store.prototype.meta)



# <a name="apidoc.module.agenda-ui"></a>[module agenda-ui](#apidoc.module.agenda-ui)

#### <a name="apidoc.element.agenda-ui.store"></a>[function <span class="apidocSignatureSpan">agenda-ui.</span>store (agenda)](#apidoc.element.agenda-ui.store)
- description and source-code
```javascript
store = function (agenda) {
  this.agenda = agenda;
  this.db = agenda._db;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.agenda-ui.store"></a>[module agenda-ui.store](#apidoc.module.agenda-ui.store)

#### <a name="apidoc.element.agenda-ui.store.store"></a>[function <span class="apidocSignatureSpan">agenda-ui.</span>store (agenda)](#apidoc.element.agenda-ui.store.store)
- description and source-code
```javascript
store = function (agenda) {
  this.agenda = agenda;
  this.db = agenda._db;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.agenda-ui.store.prototype"></a>[module agenda-ui.store.prototype](#apidoc.module.agenda-ui.store.prototype)

#### <a name="apidoc.element.agenda-ui.store.prototype.buildQuery"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>buildQuery (queryParams)](#apidoc.element.agenda-ui.store.prototype.buildQuery)
- description and source-code
```javascript
buildQuery = function (queryParams) {
  queryParams || (queryParams = {});
  var query = {};
  var filter = queryParams.filter;
  var name = queryParams.name;

  if (!filter || 'future' === filter) {
    query.nextRunAt =  { $gte: new Date() };
  } else if ('completed' === filter) {
    query.lastFinishedAt =  { $exists: true };
    query.type = 'normal';
  } else if ('failed' === filter) {
    query.failedAt =  { $exists: true };
  }

  if (name && 'All' !== name) {
    query.name = name;
  }

  return query;
}
```
- example usage
```shell
...
  jobs: this.jobs(query)
, meta: this.meta()
, definitions: this.definitions(query)
});
};

Store.prototype.jobs = function (query) {
query = this.buildQuery(query);
var jobs = RSVP.denodeify(this.agenda.jobs.bind(this.agenda));
return jobs(query).then(function (results) {
  return results.map(function (result) {
    result.attrs.jobData = result.attrs.data;
    delete result.attrs.data;
    return result;
  });
...
```

#### <a name="apidoc.element.agenda-ui.store.prototype.count"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>count (options)](#apidoc.element.agenda-ui.store.prototype.count)
- description and source-code
```javascript
count = function (options) {
  var count = RSVP.denodeify(this.db.count.bind(this.db));
  return count(this.buildQuery(options));
}
```
- example usage
```shell
...
      return result;
    });
  });
};

Store.prototype.meta = function () {
  var hash = {
    total: this.count()
  , completed: this.count({filter: 'completed'})
  , future: this.count({filter: 'future'})
  , failed: this.count({filter: 'failed'})
  };

  return RSVP.hash(hash);
};
...
```

#### <a name="apidoc.element.agenda-ui.store.prototype.data"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>data (query)](#apidoc.element.agenda-ui.store.prototype.data)
- description and source-code
```javascript
data = function (query) {
  return RSVP.hash({
    jobs: this.jobs(query)
  , meta: this.meta()
  , definitions: this.definitions(query)
  });
}
```
- example usage
```shell
...
var Store = require('./store');

module.exports = function (agenda) {
var router = express.Router();
var store = new Store(agenda);

router.get('/jobs', function (req, res) {
  store.data(req.query).then(res.json.bind(res));
});

router.get('/definitions', function (req, res) {
  store.definitions().then(function (definitions) {
    res.json({ definitions: definitions });
  });
});
...
```

#### <a name="apidoc.element.agenda-ui.store.prototype.definitionObjects"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>definitionObjects ()](#apidoc.element.agenda-ui.store.prototype.definitionObjects)
- description and source-code
```javascript
definitionObjects = function () {
  var objects = Object.keys(this.agenda._definitions).map(function (d) {
    var id = slug(d);
    return {
      _id: id
    , name: d
    , sortValue: 0
    };
  });

  objects.push({
    _id: 'all'
  , name: 'All'
  , sortValue: -1
  });

  return objects;
}
```
- example usage
```shell
...
return query;
};

Store.prototype.definitions = function (query) {
query || (query = {});
var hash = { all: this.count({filter: query.filter}) };
var indexMap = {};
var objects = this.definitionObjects();

objects.forEach(function (definition) {
  indexMap[definition._id] = objects.indexOf(definition);
  hash[definition._id] = this.count({name: definition.name, filter: query.filter});
}, this);

return RSVP.hash(hash).then(function (counts) {
...
```

#### <a name="apidoc.element.agenda-ui.store.prototype.definitions"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>definitions (query)](#apidoc.element.agenda-ui.store.prototype.definitions)
- description and source-code
```javascript
definitions = function (query) {
  query || (query = {});
  var hash = { all: this.count({filter: query.filter}) };
  var indexMap = {};
  var objects = this.definitionObjects();

  objects.forEach(function (definition) {
    indexMap[definition._id] = objects.indexOf(definition);
    hash[definition._id] = this.count({name: definition.name, filter: query.filter});
  }, this);

  return RSVP.hash(hash).then(function (counts) {
    return Object.keys(counts).map(function (id) {
      var object = objects[indexMap[id]];
      object.count = counts[id];
      return object;
    });
  });
}
```
- example usage
```shell
...
  var store = new Store(agenda);

  router.get('/jobs', function (req, res) {
    store.data(req.query).then(res.json.bind(res));
  });

  router.get('/definitions', function (req, res) {
    store.definitions().then(function (definitions) {
      res.json({ definitions: definitions });
    });
  });

  return router;
};
...
```

#### <a name="apidoc.element.agenda-ui.store.prototype.jobs"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>jobs (query)](#apidoc.element.agenda-ui.store.prototype.jobs)
- description and source-code
```javascript
jobs = function (query) {
  query = this.buildQuery(query);
  var jobs = RSVP.denodeify(this.agenda.jobs.bind(this.agenda));
  return jobs(query).then(function (results) {
    return results.map(function (result) {
      result.attrs.jobData = result.attrs.data;
      delete result.attrs.data;
      return result;
    });
  });
}
```
- example usage
```shell
...
var Store = module.exports = function (agenda) {
this.agenda = agenda;
this.db = agenda._db;
};

Store.prototype.data = function (query) {
return RSVP.hash({
  jobs: this.jobs(query)
, meta: this.meta()
, definitions: this.definitions(query)
});
};

Store.prototype.jobs = function (query) {
query = this.buildQuery(query);
...
```

#### <a name="apidoc.element.agenda-ui.store.prototype.meta"></a>[function <span class="apidocSignatureSpan">agenda-ui.store.prototype.</span>meta ()](#apidoc.element.agenda-ui.store.prototype.meta)
- description and source-code
```javascript
meta = function () {
  var hash = {
    total: this.count()
  , completed: this.count({filter: 'completed'})
  , future: this.count({filter: 'future'})
  , failed: this.count({filter: 'failed'})
  };

  return RSVP.hash(hash);
}
```
- example usage
```shell
...
this.agenda = agenda;
this.db = agenda._db;
};

Store.prototype.data = function (query) {
return RSVP.hash({
  jobs: this.jobs(query)
, meta: this.meta()
, definitions: this.definitions(query)
});
};

Store.prototype.jobs = function (query) {
query = this.buildQuery(query);
var jobs = RSVP.denodeify(this.agenda.jobs.bind(this.agenda));
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
