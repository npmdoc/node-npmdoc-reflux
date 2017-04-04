# api documentation for  [reflux (v6.4.1)](https://github.com/reflux/refluxjs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-reflux.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-reflux) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-reflux.svg)](https://travis-ci.org/npmdoc/node-npmdoc-reflux)
#### A simple library for uni-directional dataflow application architecture inspired by ReactJS Flux

[![NPM](https://nodei.co/npm/reflux.png?downloads=true)](https://www.npmjs.com/package/reflux)

[![apidoc](https://npmdoc.github.io/node-npmdoc-reflux/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-reflux_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-reflux/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-reflux/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-reflux/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mikael Brassman"
    },
    "bugs": {
        "url": "https://github.com/reflux/refluxjs/issues"
    },
    "dependencies": {
        "eventemitter3": "^1.1.1",
        "reflux-core": "^1.0.0"
    },
    "description": "A simple library for uni-directional dataflow application architecture inspired by ReactJS Flux",
    "devDependencies": {
        "benchmark": "^1.0.0",
        "browserify": "~10.2.3",
        "chai": "latest",
        "chai-as-promised": "latest",
        "es6-promise": "^2.3.0",
        "grunt": "^0.4.5",
        "grunt-browserify": "3.8.0",
        "grunt-cli": "^0.1.13",
        "grunt-contrib-jshint": "^0.11.2",
        "grunt-contrib-uglify": "^0.5.0",
        "grunt-contrib-watch": "^0.6.1",
        "grunt-karma": "latest",
        "grunt-mocha-test": "~0.12.7",
        "karma": "latest",
        "karma-browserify": "latest",
        "karma-commonjs": "latest",
        "karma-mocha": "latest",
        "karma-phantomjs-launcher": "latest",
        "karma-sauce-launcher": "latest",
        "karma-spec-reporter": "latest",
        "matchdep": "^0.3.0",
        "mocha": "latest",
        "q": "^1.0.1",
        "react-dom": "^15.0.2",
        "sinon": "^1.10.3"
    },
    "directories": {},
    "dist": {
        "shasum": "8bbbabaff54cf1b82233d67dd2542fdad2a8d678",
        "tarball": "https://registry.npmjs.org/reflux/-/reflux-6.4.1.tgz"
    },
    "gitHead": "8f40fb8cf45c133af855459d9e425cb744ad77da",
    "homepage": "https://github.com/reflux/refluxjs#readme",
    "keywords": [
        "reflux",
        "react",
        "flux",
        "architecture",
        "dataflow",
        "action",
        "event",
        "data"
    ],
    "license": "BSD-3-Clause",
    "main": "src/index.js",
    "maintainers": [
        {
            "name": "bryangrezeszak",
            "email": "bryangrezeszak@mail.com"
        },
        {
            "name": "devinivy",
            "email": "devin@bigroomstudios.com"
        },
        {
            "name": "spoike",
            "email": "mishakun+npm@gmail.com"
        }
    ],
    "name": "reflux",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^15.0.2"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/reflux/refluxjs.git"
    },
    "scripts": {
        "benchmark": "node test/benchmarks",
        "build": "grunt build",
        "test": "grunt test",
        "test:sauce": "grunt karma:sauce"
    },
    "version": "6.4.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module reflux](#apidoc.module.reflux)
1.  boolean <span class="apidocSignatureSpan">reflux.</span>serverMode
1.  [function <span class="apidocSignatureSpan">reflux.</span>Component (props, context, updater)](#apidoc.element.reflux.Component)
1.  [function <span class="apidocSignatureSpan">reflux.</span>PureComponent (props, context, updater)](#apidoc.element.reflux.PureComponent)
1.  [function <span class="apidocSignatureSpan">reflux.</span>Store ()](#apidoc.element.reflux.Store)
1.  [function <span class="apidocSignatureSpan">reflux.</span>all ()](#apidoc.element.reflux.all)
1.  [function <span class="apidocSignatureSpan">reflux.</span>connect (listenable, key)](#apidoc.element.reflux.connect)
1.  [function <span class="apidocSignatureSpan">reflux.</span>connectFilter (listenable, key, filterFunc)](#apidoc.element.reflux.connectFilter)
1.  [function <span class="apidocSignatureSpan">reflux.</span>createAction (definition)](#apidoc.element.reflux.createAction)
1.  [function <span class="apidocSignatureSpan">reflux.</span>createActions (definitions)](#apidoc.element.reflux.createActions)
1.  [function <span class="apidocSignatureSpan">reflux.</span>createStore (definition)](#apidoc.element.reflux.createStore)
1.  [function <span class="apidocSignatureSpan">reflux.</span>defineReact (react, noLongerUsed, extend)](#apidoc.element.reflux.defineReact)
1.  [function <span class="apidocSignatureSpan">reflux.</span>getGlobalState ()](#apidoc.element.reflux.getGlobalState)
1.  [function <span class="apidocSignatureSpan">reflux.</span>initStore (str)](#apidoc.element.reflux.initStore)
1.  [function <span class="apidocSignatureSpan">reflux.</span>initializeGlobalStore (str)](#apidoc.element.reflux.initializeGlobalStore)
1.  [function <span class="apidocSignatureSpan">reflux.</span>joinConcat ()](#apidoc.element.reflux.joinConcat)
1.  [function <span class="apidocSignatureSpan">reflux.</span>joinLeading ()](#apidoc.element.reflux.joinLeading)
1.  [function <span class="apidocSignatureSpan">reflux.</span>joinStrict ()](#apidoc.element.reflux.joinStrict)
1.  [function <span class="apidocSignatureSpan">reflux.</span>joinTrailing ()](#apidoc.element.reflux.joinTrailing)
1.  [function <span class="apidocSignatureSpan">reflux.</span>listenTo (listenable, callback, initial)](#apidoc.element.reflux.listenTo)
1.  [function <span class="apidocSignatureSpan">reflux.</span>listenToMany (listenables)](#apidoc.element.reflux.listenToMany)
1.  [function <span class="apidocSignatureSpan">reflux.</span>nextTick (nextTick)](#apidoc.element.reflux.nextTick)
1.  [function <span class="apidocSignatureSpan">reflux.</span>setEventEmitter (ctx)](#apidoc.element.reflux.setEventEmitter)
1.  [function <span class="apidocSignatureSpan">reflux.</span>setGlobalState (obj)](#apidoc.element.reflux.setGlobalState)
1.  [function <span class="apidocSignatureSpan">reflux.</span>use (pluginCb)](#apidoc.element.reflux.use)
1.  [function <span class="apidocSignatureSpan">reflux.</span>utils.EventEmitter ()](#apidoc.element.reflux.utils.EventEmitter)
1.  object <span class="apidocSignatureSpan">reflux.</span>ActionMethods
1.  object <span class="apidocSignatureSpan">reflux.</span>Component.prototype
1.  object <span class="apidocSignatureSpan">reflux.</span>GlobalState
1.  object <span class="apidocSignatureSpan">reflux.</span>ListenerMethods
1.  object <span class="apidocSignatureSpan">reflux.</span>ListenerMixin
1.  object <span class="apidocSignatureSpan">reflux.</span>PublisherMethods
1.  object <span class="apidocSignatureSpan">reflux.</span>PureComponent.prototype
1.  object <span class="apidocSignatureSpan">reflux.</span>Store.prototype
1.  object <span class="apidocSignatureSpan">reflux.</span>StoreMethods
1.  object <span class="apidocSignatureSpan">reflux.</span>__keep
1.  object <span class="apidocSignatureSpan">reflux.</span>stores
1.  object <span class="apidocSignatureSpan">reflux.</span>utils
1.  object <span class="apidocSignatureSpan">reflux.</span>utils.EventEmitter.prototype
1.  object <span class="apidocSignatureSpan">reflux.</span>version

#### [module reflux.Component](#apidoc.module.reflux.Component)
1.  [function <span class="apidocSignatureSpan">reflux.</span>Component (props, context, updater)](#apidoc.element.reflux.Component.Component)
1.  [function <span class="apidocSignatureSpan">reflux.Component.</span>extend (clss)](#apidoc.element.reflux.Component.extend)

#### [module reflux.Component.prototype](#apidoc.module.reflux.Component.prototype)
1.  [function <span class="apidocSignatureSpan">reflux.Component.prototype.</span>componentWillMount ()](#apidoc.element.reflux.Component.prototype.componentWillMount)
1.  [function <span class="apidocSignatureSpan">reflux.Component.prototype.</span>componentWillUnmount ()](#apidoc.element.reflux.Component.prototype.componentWillUnmount)
1.  [function <span class="apidocSignatureSpan">reflux.Component.prototype.</span>mapStoreToState (store, filterFunc)](#apidoc.element.reflux.Component.prototype.mapStoreToState)
1.  object <span class="apidocSignatureSpan">reflux.Component.prototype.</span>storeKeys

#### [module reflux.ListenerMethods](#apidoc.module.reflux.ListenerMethods)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>fetchInitialState (listenable, defaultCallback)](#apidoc.element.reflux.ListenerMethods.fetchInitialState)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>hasListener (listenable)](#apidoc.element.reflux.ListenerMethods.hasListener)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinConcat ()](#apidoc.element.reflux.ListenerMethods.joinConcat)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinLeading ()](#apidoc.element.reflux.ListenerMethods.joinLeading)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinStrict ()](#apidoc.element.reflux.ListenerMethods.joinStrict)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinTrailing ()](#apidoc.element.reflux.ListenerMethods.joinTrailing)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>listenTo (listenable, callback, defaultCallback)](#apidoc.element.reflux.ListenerMethods.listenTo)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>listenToMany (listenables)](#apidoc.element.reflux.ListenerMethods.listenToMany)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>stopListeningTo (listenable)](#apidoc.element.reflux.ListenerMethods.stopListeningTo)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>stopListeningToAll ()](#apidoc.element.reflux.ListenerMethods.stopListeningToAll)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>validateListening (listenable)](#apidoc.element.reflux.ListenerMethods.validateListening)

#### [module reflux.ListenerMixin](#apidoc.module.reflux.ListenerMixin)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>componentWillUnmount ()](#apidoc.element.reflux.ListenerMixin.componentWillUnmount)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>fetchInitialState (listenable, defaultCallback)](#apidoc.element.reflux.ListenerMixin.fetchInitialState)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>hasListener (listenable)](#apidoc.element.reflux.ListenerMixin.hasListener)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinConcat ()](#apidoc.element.reflux.ListenerMixin.joinConcat)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinLeading ()](#apidoc.element.reflux.ListenerMixin.joinLeading)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinStrict ()](#apidoc.element.reflux.ListenerMixin.joinStrict)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinTrailing ()](#apidoc.element.reflux.ListenerMixin.joinTrailing)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>listenTo (listenable, callback, defaultCallback)](#apidoc.element.reflux.ListenerMixin.listenTo)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>listenToMany (listenables)](#apidoc.element.reflux.ListenerMixin.listenToMany)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>stopListeningTo (listenable)](#apidoc.element.reflux.ListenerMixin.stopListeningTo)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>stopListeningToAll ()](#apidoc.element.reflux.ListenerMixin.stopListeningToAll)
1.  [function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>validateListening (listenable)](#apidoc.element.reflux.ListenerMixin.validateListening)

#### [module reflux.PublisherMethods](#apidoc.module.reflux.PublisherMethods)
1.  [function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>deferWith (callback)](#apidoc.element.reflux.PublisherMethods.deferWith)
1.  [function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>listen (callback, bindContext)](#apidoc.element.reflux.PublisherMethods.listen)
1.  [function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>preEmit ()](#apidoc.element.reflux.PublisherMethods.preEmit)
1.  [function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>shouldEmit ()](#apidoc.element.reflux.PublisherMethods.shouldEmit)
1.  [function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>trigger ()](#apidoc.element.reflux.PublisherMethods.trigger)
1.  [function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>triggerAsync ()](#apidoc.element.reflux.PublisherMethods.triggerAsync)

#### [module reflux.PureComponent](#apidoc.module.reflux.PureComponent)
1.  [function <span class="apidocSignatureSpan">reflux.</span>PureComponent (props, context, updater)](#apidoc.element.reflux.PureComponent.PureComponent)
1.  [function <span class="apidocSignatureSpan">reflux.PureComponent.</span>extend (clss)](#apidoc.element.reflux.PureComponent.extend)

#### [module reflux.PureComponent.prototype](#apidoc.module.reflux.PureComponent.prototype)
1.  [function <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>componentWillMount ()](#apidoc.element.reflux.PureComponent.prototype.componentWillMount)
1.  [function <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>componentWillUnmount ()](#apidoc.element.reflux.PureComponent.prototype.componentWillUnmount)
1.  [function <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>mapStoreToState (store, filterFunc)](#apidoc.element.reflux.PureComponent.prototype.mapStoreToState)
1.  object <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>storeKeys

#### [module reflux.Store](#apidoc.module.reflux.Store)
1.  boolean <span class="apidocSignatureSpan">reflux.Store.</span>isES6Store
1.  [function <span class="apidocSignatureSpan">reflux.</span>Store ()](#apidoc.element.reflux.Store.Store)

#### [module reflux.Store.prototype](#apidoc.module.reflux.Store.prototype)
1.  [function <span class="apidocSignatureSpan">reflux.Store.prototype.</span>setState (obj)](#apidoc.element.reflux.Store.prototype.setState)

#### [module reflux.__keep](#apidoc.module.reflux.__keep)
1.  [function <span class="apidocSignatureSpan">reflux.__keep.</span>addAction (act)](#apidoc.element.reflux.__keep.addAction)
1.  [function <span class="apidocSignatureSpan">reflux.__keep.</span>addStore (str)](#apidoc.element.reflux.__keep.addStore)
1.  [function <span class="apidocSignatureSpan">reflux.__keep.</span>reset ()](#apidoc.element.reflux.__keep.reset)
1.  [function <span class="apidocSignatureSpan">reflux.__keep.</span>useKeep ()](#apidoc.element.reflux.__keep.useKeep)
1.  object <span class="apidocSignatureSpan">reflux.__keep.</span>createdActions
1.  object <span class="apidocSignatureSpan">reflux.__keep.</span>createdStores

#### [module reflux.utils](#apidoc.module.reflux.utils)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>EventEmitter ()](#apidoc.element.reflux.utils.EventEmitter)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>callbackName (string, prefix)](#apidoc.element.reflux.utils.callbackName)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>capitalize (string)](#apidoc.element.reflux.utils.capitalize)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>extend (obj)](#apidoc.element.reflux.utils.extend)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>inherits (subClass, superClass)](#apidoc.element.reflux.utils.inherits)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>isArguments (value)](#apidoc.element.reflux.utils.isArguments)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>isFunction (value)](#apidoc.element.reflux.utils.isFunction)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>isObject (obj)](#apidoc.element.reflux.utils.isObject)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>nextTick (callback)](#apidoc.element.reflux.utils.nextTick)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>object (keys, vals)](#apidoc.element.reflux.utils.object)
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>throwIf (val, msg)](#apidoc.element.reflux.utils.throwIf)

#### [module reflux.utils.EventEmitter](#apidoc.module.reflux.utils.EventEmitter)
1.  boolean <span class="apidocSignatureSpan">reflux.utils.EventEmitter.</span>prefixed
1.  [function <span class="apidocSignatureSpan">reflux.utils.</span>EventEmitter ()](#apidoc.element.reflux.utils.EventEmitter.EventEmitter)

#### [module reflux.utils.EventEmitter.prototype](#apidoc.module.reflux.utils.EventEmitter.prototype)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>addListener (event, fn, context)](#apidoc.element.reflux.utils.EventEmitter.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>emit (event, a1, a2, a3, a4, a5)](#apidoc.element.reflux.utils.EventEmitter.prototype.emit)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>eventNames ()](#apidoc.element.reflux.utils.EventEmitter.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>listeners (event, exists)](#apidoc.element.reflux.utils.EventEmitter.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>off (event, fn, context, once)](#apidoc.element.reflux.utils.EventEmitter.prototype.off)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>on (event, fn, context)](#apidoc.element.reflux.utils.EventEmitter.prototype.on)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>once (event, fn, context)](#apidoc.element.reflux.utils.EventEmitter.prototype.once)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>removeAllListeners (event)](#apidoc.element.reflux.utils.EventEmitter.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>removeListener (event, fn, context, once)](#apidoc.element.reflux.utils.EventEmitter.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>setMaxListeners ()](#apidoc.element.reflux.utils.EventEmitter.prototype.setMaxListeners)



# <a name="apidoc.module.reflux"></a>[module reflux](#apidoc.module.reflux)

#### <a name="apidoc.element.reflux.Component"></a>[function <span class="apidocSignatureSpan">reflux.</span>Component (props, context, updater)](#apidoc.element.reflux.Component)
- description and source-code
```javascript
Component = function (props, context, updater) {
		_extend.call(this, props, context, updater);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PureComponent"></a>[function <span class="apidocSignatureSpan">reflux.</span>PureComponent (props, context, updater)](#apidoc.element.reflux.PureComponent)
- description and source-code
```javascript
PureComponent = function (props, context, updater) {
		_extend.call(this, props, context, updater);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.Store"></a>[function <span class="apidocSignatureSpan">reflux.</span>Store ()](#apidoc.element.reflux.Store)
- description and source-code
```javascript
Store = function () {
		// extending doesn't really work well here, so instead we create an internal instance
		// and just loop through its properties/methods and make a getter/setter for each
		// that will actually be getting and setting on that internal instance.
		this.__store__ = Reflux.createStore();
		this.state = {};
		var self = this;
		for (var key in this.__store__) {
			/*jshint loopfunc: true */
			(function (prop) {
				Object.defineProperty(self, prop, {
					get: function () { return self.__store__[prop]; },
					set: function (v) { self.__store__[prop] = v; }
				});
			})(key);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.all"></a>[function <span class="apidocSignatureSpan">reflux.</span>all ()](#apidoc.element.reflux.all)
- description and source-code
```javascript
all = function () /* listenables... */{
    var listenables = slice.call(arguments);
    return (0, _createStore.createStore)({
        init: function init() {
            this[strategyMethodNames[strategy]].apply(this, listenables.concat("triggerAsync"));
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.connect"></a>[function <span class="apidocSignatureSpan">reflux.</span>connect (listenable, key)](#apidoc.element.reflux.connect)
- description and source-code
```javascript
connect = function (listenable, key) {

    _.throwIf(typeof(key) === 'undefined', 'Reflux.connect() requires a key.');

    return {
        getInitialState: function() {
            if (!_.isFunction(listenable.getInitialState)) {
                return {};
            }

            return _.object([key],[listenable.getInitialState()]);
        },
        componentDidMount: function() {
            var me = this;

            _.extend(me, ListenerMethods);

            this.listenTo(listenable, function(v) {
                me.setState(_.object([key],[v]));
            });
        },
        componentWillUnmount: ListenerMixin.componentWillUnmount
    };
}
```
- example usage
```shell
...

var ListenerMethods = require('reflux-core/lib/ListenerMethods'),
ListenerMixin = require('./ListenerMixin'),
_ = require('reflux-core/lib/utils');

module.exports = function(listenable, key) {

_.throwIf(typeof(key) === 'undefined', 'Reflux.connect() requires a key.');

return {
    getInitialState: function() {
        if (!_.isFunction(listenable.getInitialState)) {
            return {};
        }
...
```

#### <a name="apidoc.element.reflux.connectFilter"></a>[function <span class="apidocSignatureSpan">reflux.</span>connectFilter (listenable, key, filterFunc)](#apidoc.element.reflux.connectFilter)
- description and source-code
```javascript
connectFilter = function (listenable, key, filterFunc) {

    _.throwIf(_.isFunction(key), 'Reflux.connectFilter() requires a key.');

    return {
        getInitialState: function() {
            if (!_.isFunction(listenable.getInitialState)) {
                return {};
            }

            // Filter initial payload from store.
            var result = filterFunc.call(this, listenable.getInitialState());
            if (typeof(result) !== 'undefined') {
                return _.object([key], [result]);
            } else {
                return {};
            }
        },
        componentDidMount: function() {
            var me = this;

            _.extend(this, ListenerMethods);

            this.listenTo(listenable, function(value) {
                var result = filterFunc.call(me, value);
                me.setState(_.object([key], [result]));
            });
        },
        componentWillUnmount: ListenerMixin.componentWillUnmount
    };
}
```
- example usage
```shell
...

var ListenerMethods = require('reflux-core/lib/ListenerMethods'),
ListenerMixin = require('./ListenerMixin'),
_ = require('reflux-core/lib/utils');

module.exports = function(listenable, key, filterFunc) {

_.throwIf(_.isFunction(key), 'Reflux.connectFilter() requires a key.');

return {
    getInitialState: function() {
        if (!_.isFunction(listenable.getInitialState)) {
            return {};
        }
...
```

#### <a name="apidoc.element.reflux.createAction"></a>[function <span class="apidocSignatureSpan">reflux.</span>createAction (definition)](#apidoc.element.reflux.createAction)
- description and source-code
```javascript
function createAction(definition) {

    definition = definition || {};
    if (!_.isObject(definition)) {
        definition = { actionName: definition };
    }

    for (var a in ActionMethods) {
        if (!allowed[a] && PublisherMethods[a]) {
            throw new Error("Cannot override API method " + a + " in Reflux.ActionMethods. Use another method name or override it
 on Reflux.PublisherMethods instead.");
        }
    }

    for (var d in definition) {
        if (!allowed[d] && PublisherMethods[d]) {
            throw new Error("Cannot override API method " + d + " in action creation. Use another method name or override it on
Reflux.PublisherMethods instead.");
        }
    }

    definition.children = definition.children || [];
    if (definition.asyncResult) {
        definition.children = definition.children.concat(["completed", "failed"]);
    }

    var i = 0,
        childActions = {};
    for (; i < definition.children.length; i++) {
        var chDef = definition.children[i];
        var chName = typeof chDef === "string" ? chDef : chDef.actionName;
        childActions[chName] = createAction(chDef);
    }

    var context = _.extend({
        eventLabel: "action",
        emitter: new _.EventEmitter(),
        _isAction: true
    }, PublisherMethods, ActionMethods, definition);

    var functor = function functor() {
        var hasChildActions = false;
<span class="apidocCodeCommentSpan">        /* eslint no-unused-vars:0 */
</span>        for (var ignore in functor.childActions) {
            hasChildActions = true;break;
        }
        var async = !functor.sync && typeof functor.sync !== "undefined" || hasChildActions;
        var triggerType = async ? "triggerAsync" : "trigger";
        return functor[triggerType].apply(functor, arguments);
    };

    _.extend(functor, childActions, context);

    Keep.addAction(functor);

    return functor;
}
```
- example usage
```shell
...
--------------------------------

## Creating Actions

Create an action by calling 'Reflux.createAction' with an optional options object.

'''javascript
var statusUpdate = Reflux.createAction();
'''

An action is a [function object](http://en.wikipedia.org/wiki/Function_object) that can be invoked like any other function.

'''javascript
statusUpdate(data); // Invokes the action statusUpdate
'''
...
```

#### <a name="apidoc.element.reflux.createActions"></a>[function <span class="apidocSignatureSpan">reflux.</span>createActions (definitions)](#apidoc.element.reflux.createActions)
- description and source-code
```javascript
createActions = function (definitions) {
    var actions = {};
    if (definitions instanceof Array) {
        definitions.forEach(function (val) {
            if (_.isObject(val)) {
                reducer(val, actions);
            } else {
                actions[val] = (0, _createAction.createAction)(val);
            }
        });
    } else {
        reducer(definitions, actions);
    }
    return actions;
}
```
- example usage
```shell
...
'''javascript
statusUpdate(data); // Invokes the action statusUpdate
'''

There is also a convenience function for creating multiple actions.

'''javascript
var Actions = Reflux.createActions([
    "statusUpdate",
    "statusEdited",
    "statusAdded"
]);

// Actions object now contains the actions
// with the names given in the array above
...
```

#### <a name="apidoc.element.reflux.createStore"></a>[function <span class="apidocSignatureSpan">reflux.</span>createStore (definition)](#apidoc.element.reflux.createStore)
- description and source-code
```javascript
function createStore(definition) {

    definition = definition || {};

    for (var a in StoreMethods) {
        if (!allowed[a] && (PublisherMethods[a] || ListenerMethods[a])) {
            throw new Error("Cannot override API method " + a + " in Reflux.StoreMethods. Use another method name or override it
 on Reflux.PublisherMethods / Reflux.ListenerMethods instead.");
        }
    }

    for (var d in definition) {
        if (!allowed[d] && (PublisherMethods[d] || ListenerMethods[d])) {
            throw new Error("Cannot override API method " + d + " in store creation. Use another method name or override it on Reflux
.PublisherMethods / Reflux.ListenerMethods instead.");
        }
    }

    definition = (0, _mixer.mix)(definition);

    function Store() {
        var i = 0,
            arr;
        this.subscriptions = [];
        this.emitter = new _.EventEmitter();
        this.eventLabel = "change";
        (0, _bindMethods.bindMethods)(this, definition);
        if (this.init && _.isFunction(this.init)) {
            this.init();
        }
        if (this.listenables) {
            arr = [].concat(this.listenables);
            for (; i < arr.length; i++) {
                this.listenToMany(arr[i]);
            }
        }
    }

    _.extend(Store.prototype, ListenerMethods, PublisherMethods, StoreMethods, definition);

    var store = new Store();
    Keep.addStore(store);

    return store;
}
```
- example usage
```shell
...
	 * with this.store or this.stores in an ES6 component just plass the class,
	 * it will deal with a singleton instantiation of the class automatically.
	 */
	var RefluxStore = function() {
		// extending doesn't really work well here, so instead we create an internal instance
		// and just loop through its properties/methods and make a getter/setter for each
		// that will actually be getting and setting on that internal instance.
		this.__store__ = Reflux.createStore();
		this.state = {};
		var self = this;
		for (var key in this.__store__) {
			/*jshint loopfunc: true */
			(function (prop) {
				Object.defineProperty(self, prop, {
					get: function () { return self.__store__[prop]; },
...
```

#### <a name="apidoc.element.reflux.defineReact"></a>[function <span class="apidocSignatureSpan">reflux.</span>defineReact (react, noLongerUsed, extend)](#apidoc.element.reflux.defineReact)
- description and source-code
```javascript
function defineReact(react, noLongerUsed, extend)
{
	var proto, _extend;
	
	// if no Reflux object is yet available then return and just wait until defineReact is called manually with it
	try {
		_react  = react  || _react  || React;
		_extend = extend || _react.Component;
	} catch (e) {
		return;
	}
	
	// if Reflux and React aren't present then ignore, wait until they are properly present
	// also ignore if it's been called before UNLESS there's manual extending happening
	if (!_react || !_extend || (_defined && !extend)) {
		return;
	}
	
	// ----------- BEGIN Reflux.Component ------------
	/**
	 * Reflux.Component:
	 * An implementation for idiomatic React.js classes that mix with
	 * Reflux stores. To utilize extend Reflux.Component instead of
	 * React.Component. Then you may hook any Reflux store that has a
	 * 'this.state' property containing its state values to the component
	 * via 'this.store' or an Array of Reflux stores via 'this.stores' in
	 * the component's constructor (similar to how you assign initial state
	 * in the constructor in ES6 style React). The default values of the
	 * stores will automatically reflect in the component's state, and any
	 * further 'trigger' calls from that store will update properties passed
	 * in the trigger into the component automatically.
	 */
	var RefluxComponent = function(props, context, updater) {
		_extend.call(this, props, context, updater);
	};
	
	// equivalent of 'extends React.Component' or other class if provided via 'extend' param
	Reflux.utils.inherits(RefluxComponent, _extend);
	
	proto = RefluxComponent.prototype;
	
	/**
	 * this.storeKeys
	 * When this is a falsey value (null by default) the component mixes in
	 * all properties from the stores attached to it and updates on changes
	 * from all of them. When set to an array of string keys it will only
	 * utilized state property names of those keys in any store attached. This
	 * lets you choose which parts of stores update the component on a component-
	 * by-component basis. If using this it is best set in the constructor.
	 */
	proto.storeKeys = null;
	
	// on the mounting of the component that is where the store/stores are attached and initialized if needed
	proto.componentWillMount = function () {
		// if there is a this.store then simply push it onto the this.stores array or make one if needed
		if (this.store) {
			if (Array.isArray(this.stores)) {
				this.stores.unshift(this.store);
			} else {
				this.stores = [this.store];
			}
		}
		
		if (this.stores) {
			this.__storeunsubscribes__ = this.__storeunsubscribes__ || [];
			var sS = this.setState.bind(this);
			// this handles the triggering of a store, checking what's updated if proto.storeKeys is utilized
			var onStoreTrigger = function(obj){
				var updateObj = filterByStoreKeys(this.storeKeys, obj);
				if (updateObj) {
					sS(updateObj);
				}
			}.bind(this);
			// for each store in this.stores...
			for (var i = 0, ii = this.stores.length; i < ii; i++) {
				var str = this.stores[i];
				// if's a function then we know it's a class getting passed, not an instance
				if (typeof str === 'function') {
					var storeId = str.id;
					// if there is NOT a .singleton property on the store then this store has not been initialized yet, so do so
					if (!str.singleton) {
						str.singleton = new str();
						if (storeId) {
							Reflux.stores[storeId] = str.singleton;
						}
					}
					// before we weren't sure if we were working with an instance or class, so now we know an instance is created set it
					// to the variables we were using so that we can just continue on knowing it's the instance we're working with
					this.stores[i] = str = str.singleton;
					// the instance should have an .id property as well if the class does, so set that here
					str.id = storeId;
					// if there is an id and there is a global state property for this store then merge
					// the properties from that global state into the default state of the store AND then ...
```
- example usage
```shell
...
			subClass.__proto__ = superClass;
		}
	}
};

// first try to see if there's a global React var and use it
if (typeof React !== 'undefined' && React) {
	Reflux.defineReact(React);
// otherwise we're gonna resort to 'try' stuff in case of other environments
} else {
	try {
		var R = require("react"); // we ignore this in browserify manually (see grunt file), so it's more of a doublecheck for in node
		Reflux.defineReact(R);
	} catch (e) {}
}
...
```

#### <a name="apidoc.element.reflux.getGlobalState"></a>[function <span class="apidocSignatureSpan">reflux.</span>getGlobalState ()](#apidoc.element.reflux.getGlobalState)
- description and source-code
```javascript
getGlobalState = function () {
		return clone(Reflux.GlobalState);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.initStore"></a>[function <span class="apidocSignatureSpan">reflux.</span>initStore (str)](#apidoc.element.reflux.initStore)
- description and source-code
```javascript
initStore = function (str) {
		var storeId = str.id;
		// if they're initializing something twice then we're done already, return it
		if (str.singleton) {
			return str.singleton;
		}
		// if no id then it's easy: just make new instance and set to singleton
		if (!storeId) {
			str.singleton = new str();
			return str.singleton;
		}
		// create the singleton and assign it to the class's singleton static property
		var inst = str.singleton = new str();
		// store it on the Reflux.stores array to be accessible later
		Reflux.stores[storeId] = inst;
		// the singleton instance itself should also have the id property of the class
		inst.id = storeId;
		// if the global state has something set for this id, copy it to the state and then
		// make sure to set the global state to the end result, since it may have only been partial
		if (Reflux.GlobalState[storeId]) {
			for (var key in Reflux.GlobalState[storeId]) {
				inst.state[key] = Reflux.GlobalState[storeId][key];
			}
			Reflux.GlobalState[storeId] = inst.state;
		// otherwise just set the global state to the default state of the class
		} else {
			Reflux.GlobalState[storeId] = inst.state;
		}
		// returns the singleton itself, though it will also be accessible as as 'MyClass.singleton'
		return inst;
	}
```
- example usage
```shell
...
	proto.mapStoreToState = function(store, filterFunc)
	{
		// make sure we have a proper singleton instance to work with
		if (typeof store === 'function') {
			if (store.singleton) {
				store = store.singleton;
			} else {
				store = Reflux.initStore(store);
			}
		}
		
		// we need a closure so that the called function can remember the proper filter function to use, so function gets defined here
		var self = this;
		function onMapStoreTrigger(obj) {
			// get an object
...
```

#### <a name="apidoc.element.reflux.initializeGlobalStore"></a>[function <span class="apidocSignatureSpan">reflux.</span>initializeGlobalStore (str)](#apidoc.element.reflux.initializeGlobalStore)
- description and source-code
```javascript
initializeGlobalStore = function (str) {
		var storeId = str.id;
		// if they're initializing something twice then we're done already, return it
		if (str.singleton) {
			return str.singleton;
		}
		// if no id then it's easy: just make new instance and set to singleton
		if (!storeId) {
			str.singleton = new str();
			return str.singleton;
		}
		// create the singleton and assign it to the class's singleton static property
		var inst = str.singleton = new str();
		// store it on the Reflux.stores array to be accessible later
		Reflux.stores[storeId] = inst;
		// the singleton instance itself should also have the id property of the class
		inst.id = storeId;
		// if the global state has something set for this id, copy it to the state and then
		// make sure to set the global state to the end result, since it may have only been partial
		if (Reflux.GlobalState[storeId]) {
			for (var key in Reflux.GlobalState[storeId]) {
				inst.state[key] = Reflux.GlobalState[storeId][key];
			}
			Reflux.GlobalState[storeId] = inst.state;
		// otherwise just set the global state to the default state of the class
		} else {
			Reflux.GlobalState[storeId] = inst.state;
		}
		// returns the singleton itself, though it will also be accessible as as 'MyClass.singleton'
		return inst;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.joinConcat"></a>[function <span class="apidocSignatureSpan">reflux.</span>joinConcat ()](#apidoc.element.reflux.joinConcat)
- description and source-code
```javascript
joinConcat = function () /* listenables... */{
    var listenables = slice.call(arguments);
    return (0, _createStore.createStore)({
        init: function init() {
            this[strategyMethodNames[strategy]].apply(this, listenables.concat("triggerAsync"));
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.joinLeading"></a>[function <span class="apidocSignatureSpan">reflux.</span>joinLeading ()](#apidoc.element.reflux.joinLeading)
- description and source-code
```javascript
joinLeading = function () /* listenables... */{
    var listenables = slice.call(arguments);
    return (0, _createStore.createStore)({
        init: function init() {
            this[strategyMethodNames[strategy]].apply(this, listenables.concat("triggerAsync"));
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.joinStrict"></a>[function <span class="apidocSignatureSpan">reflux.</span>joinStrict ()](#apidoc.element.reflux.joinStrict)
- description and source-code
```javascript
joinStrict = function () /* listenables... */{
    var listenables = slice.call(arguments);
    return (0, _createStore.createStore)({
        init: function init() {
            this[strategyMethodNames[strategy]].apply(this, listenables.concat("triggerAsync"));
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.joinTrailing"></a>[function <span class="apidocSignatureSpan">reflux.</span>joinTrailing ()](#apidoc.element.reflux.joinTrailing)
- description and source-code
```javascript
joinTrailing = function () /* listenables... */{
    var listenables = slice.call(arguments);
    return (0, _createStore.createStore)({
        init: function init() {
            this[strategyMethodNames[strategy]].apply(this, listenables.concat("triggerAsync"));
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.listenTo"></a>[function <span class="apidocSignatureSpan">reflux.</span>listenTo (listenable, callback, initial)](#apidoc.element.reflux.listenTo)
- description and source-code
```javascript
listenTo = function (listenable, callback, initial){
    return {
        /**
         * Set up the mixin before the initial rendering occurs. Import methods from 'ListenerMethods'
         * and then make the call to 'listenTo' with the arguments provided to the factory function
         */
        componentDidMount: function() {
            for(var m in ListenerMethods){
                if (this[m] !== ListenerMethods[m]){
                    if (this[m]){
                        throw "Can't have other property '"+m+"' when using Reflux.listenTo!";
                    }
                    this[m] = ListenerMethods[m];
                }
            }
            this.listenTo(listenable,callback,initial);
        },
        /**
         * Cleans up all listener previously registered.
         */
        componentWillUnmount: ListenerMethods.stopListeningToAll
    };
}
```
- example usage
```shell
...
'''javascript
class StatusStore extends Reflux.Store
{
constructor()
{
    super();
    this.state = {flag:'OFFLINE'}; // <- set store's default state much like in React
    this.listenTo(statusUpdate, this.onStatusUpdate); // listen to the statusUpdate action
}

onStatusUpdate(status)
{
    var newFlag = status ? 'ONLINE' : 'OFFLINE';
    this.setState({flag:newFlag});
}
...
```

#### <a name="apidoc.element.reflux.listenToMany"></a>[function <span class="apidocSignatureSpan">reflux.</span>listenToMany (listenables)](#apidoc.element.reflux.listenToMany)
- description and source-code
```javascript
listenToMany = function (listenables){
    return {
        /**
         * Set up the mixin before the initial rendering occurs. Import methods from 'ListenerMethods'
         * and then make the call to 'listenTo' with the arguments provided to the factory function
         */
        componentDidMount: function() {
            for(var m in ListenerMethods){
                if (this[m] !== ListenerMethods[m]){
                    if (this[m]){
                        throw "Can't have other property '"+m+"' when using Reflux.listenToMany!";
                    }
                    this[m] = ListenerMethods[m];
                }
            }
            this.listenToMany(listenables);
        },
        /**
         * Cleans up all listener previously registered.
         */
        componentWillUnmount: ListenerMethods.stopListeningToAll
    };
}
```
- example usage
```shell
...
						Combined[key] = obj[key];
					}
				});
			} else {
				Combined = v;
			}
			this.__listenables__ = Combined;
			this.listenToMany(Combined);
		},
		enumerable: true,
		configurable: true
	});
	
	// allows simple usage of 'this.setState(obj)' within the store to both update the state and trigger the store to update
	// components that it is attached to in a simple way that is idiomatic with React
...
```

#### <a name="apidoc.element.reflux.nextTick"></a>[function <span class="apidocSignatureSpan">reflux.</span>nextTick (nextTick)](#apidoc.element.reflux.nextTick)
- description and source-code
```javascript
function nextTick(nextTick) {
    _.nextTick = nextTick;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.setEventEmitter"></a>[function <span class="apidocSignatureSpan">reflux.</span>setEventEmitter (ctx)](#apidoc.element.reflux.setEventEmitter)
- description and source-code
```javascript
function setEventEmitter(ctx) {
    _.EventEmitter = ctx;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.setGlobalState"></a>[function <span class="apidocSignatureSpan">reflux.</span>setGlobalState (obj)](#apidoc.element.reflux.setGlobalState)
- description and source-code
```javascript
setGlobalState = function (obj) {
		for (var storeID in obj) {
			if (Reflux.stores[storeID]) {
				Reflux.stores[storeID].setState(obj[storeID]);
			} else {
				Reflux.GlobalState[storeID] = obj[storeID];
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.use"></a>[function <span class="apidocSignatureSpan">reflux.</span>use (pluginCb)](#apidoc.element.reflux.use)
- description and source-code
```javascript
function use(pluginCb) {
    pluginCb(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter"></a>[function <span class="apidocSignatureSpan">reflux.</span>utils.EventEmitter ()](#apidoc.element.reflux.utils.EventEmitter)
- description and source-code
```javascript
function EventEmitter() { /* Nothing to set */ }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.Component"></a>[module reflux.Component](#apidoc.module.reflux.Component)

#### <a name="apidoc.element.reflux.Component.Component"></a>[function <span class="apidocSignatureSpan">reflux.</span>Component (props, context, updater)](#apidoc.element.reflux.Component.Component)
- description and source-code
```javascript
Component = function (props, context, updater) {
		_extend.call(this, props, context, updater);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.Component.extend"></a>[function <span class="apidocSignatureSpan">reflux.Component.</span>extend (clss)](#apidoc.element.reflux.Component.extend)
- description and source-code
```javascript
extend = function (clss) {
		return defineReact(null, null, clss);
	}
```
- example usage
```shell
...
        }

        return _.object([key],[listenable.getInitialState()]);
    },
    componentDidMount: function() {
        var me = this;

        _.extend(me, ListenerMethods);

        this.listenTo(listenable, function(v) {
            me.setState(_.object([key],[v]));
        });
    },
    componentWillUnmount: ListenerMixin.componentWillUnmount
};
...
```



# <a name="apidoc.module.reflux.Component.prototype"></a>[module reflux.Component.prototype](#apidoc.module.reflux.Component.prototype)

#### <a name="apidoc.element.reflux.Component.prototype.componentWillMount"></a>[function <span class="apidocSignatureSpan">reflux.Component.prototype.</span>componentWillMount ()](#apidoc.element.reflux.Component.prototype.componentWillMount)
- description and source-code
```javascript
componentWillMount = function () {
		// if there is a this.store then simply push it onto the this.stores array or make one if needed
		if (this.store) {
			if (Array.isArray(this.stores)) {
				this.stores.unshift(this.store);
			} else {
				this.stores = [this.store];
			}
		}
		
		if (this.stores) {
			this.__storeunsubscribes__ = this.__storeunsubscribes__ || [];
			var sS = this.setState.bind(this);
			// this handles the triggering of a store, checking what's updated if proto.storeKeys is utilized
			var onStoreTrigger = function(obj){
				var updateObj = filterByStoreKeys(this.storeKeys, obj);
				if (updateObj) {
					sS(updateObj);
				}
			}.bind(this);
			// for each store in this.stores...
			for (var i = 0, ii = this.stores.length; i < ii; i++) {
				var str = this.stores[i];
				// if's a function then we know it's a class getting passed, not an instance
				if (typeof str === 'function') {
					var storeId = str.id;
					// if there is NOT a .singleton property on the store then this store has not been initialized yet, so do so
					if (!str.singleton) {
						str.singleton = new str();
						if (storeId) {
							Reflux.stores[storeId] = str.singleton;
						}
					}
					// before we weren't sure if we were working with an instance or class, so now we know an instance is created set it
					// to the variables we were using so that we can just continue on knowing it's the instance we're working with
					this.stores[i] = str = str.singleton;
					// the instance should have an .id property as well if the class does, so set that here
					str.id = storeId;
					// if there is an id and there is a global state property for this store then merge
					// the properties from that global state into the default state of the store AND then
					// set the global state to that new state (since it may have previously been partial)
					if (storeId && Reflux.GlobalState[storeId]) {
						for (var key in Reflux.GlobalState[storeId]) {
							str.state[key] = Reflux.GlobalState[storeId][key];
						}
						Reflux.GlobalState[storeId] = str.state;
					// otherwise (if it has an id) set the global state to the default state of the store
					} else if (storeId) {
						Reflux.GlobalState[storeId] = str.state;
					}
					// if no id, then no messing with global state
				}
				// listen/subscribe for the ".trigger()" in the store, and track the unsubscribes so that we can unsubscribe on unmount
				if (!Reflux.serverMode) {
					this.__storeunsubscribes__.push(str.listen(onStoreTrigger));
				}
				// run set state so that it mixes in the props from the store with the component
				var updateObj = filterByStoreKeys(this.storeKeys, str.state);
				if (updateObj) {
					this.setState(updateObj);
				}
			}
		}
		
		// mapStoreToState needs to know if is ready to map or must wait
		this.__readytomap__ = true;
		// if there are mappings that were delayed, do them now
		var dmaps = this.__delayedmaps__;
		if (dmaps) {
			for (var j=0,jj=dmaps.length; j<jj; j++) {
				dmaps[j].func( dmaps[j].state );
			}
		}
		this.__delayedmaps__ = null;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.Component.prototype.componentWillUnmount"></a>[function <span class="apidocSignatureSpan">reflux.Component.prototype.</span>componentWillUnmount ()](#apidoc.element.reflux.Component.prototype.componentWillUnmount)
- description and source-code
```javascript
componentWillUnmount = function () {
		if (this.__storeunsubscribes__) {
			for (var i = 0, ii = this.__storeunsubscribes__.length; i < ii; i++) {
				this.__storeunsubscribes__[i]();
			}
		}
		this.__readytomap__ = false;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.Component.prototype.mapStoreToState"></a>[function <span class="apidocSignatureSpan">reflux.Component.prototype.</span>mapStoreToState (store, filterFunc)](#apidoc.element.reflux.Component.prototype.mapStoreToState)
- description and source-code
```javascript
mapStoreToState = function (store, filterFunc)
	{
		// make sure we have a proper singleton instance to work with
		if (typeof store === 'function') {
			if (store.singleton) {
				store = store.singleton;
			} else {
				store = Reflux.initStore(store);
			}
		}
		
		// we need a closure so that the called function can remember the proper filter function to use, so function gets defined here
		var self = this;
		function onMapStoreTrigger(obj) {
			// get an object
			var update = filterFunc.call(self, obj);
			// if no object returned from filter functions do nothing
			if (!update) {
				return;
			}
			// check if the update actually has any mapped props
			/*jshint unused: false */
			var hasProps = false;
			for (var check in update) {
				hasProps = true;
				break;
			}
			// if there were props mapped, then update via setState
			if (hasProps) {
				self.setState(update);
			}
		}
		
		// add the listener to know when the store is triggered
		this.__storeunsubscribes__ = this.__storeunsubscribes__ || [];
		this.__storeunsubscribes__.push(store.listen(onMapStoreTrigger));
		
		// now actually run onMapStoreTrigger with the full store state so that we immediately have all store state mapped to component
 state
		if (this.__readytomap__) {
			onMapStoreTrigger(store.state);
		} else {
			this.__delayedmaps__ = this.__delayedmaps__ || [];
			this.__delayedmaps__.push({func:onMapStoreTrigger, state:store.state});
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.ListenerMethods"></a>[module reflux.ListenerMethods](#apidoc.module.reflux.ListenerMethods)

#### <a name="apidoc.element.reflux.ListenerMethods.fetchInitialState"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>fetchInitialState (listenable, defaultCallback)](#apidoc.element.reflux.ListenerMethods.fetchInitialState)
- description and source-code
```javascript
function fetchInitialState(listenable, defaultCallback) {
    defaultCallback = defaultCallback && this[defaultCallback] || defaultCallback;
    var me = this;
    if (_.isFunction(defaultCallback) && _.isFunction(listenable.getInitialState)) {
        var data = listenable.getInitialState();
        if (data && _.isFunction(data.then)) {
            data.then(function () {
                defaultCallback.apply(me, arguments);
            });
        } else {
            defaultCallback.call(this, data);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.hasListener"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>hasListener (listenable)](#apidoc.element.reflux.ListenerMethods.hasListener)
- description and source-code
```javascript
function hasListener(listenable) {
    var i = 0,
        j,
        listener,
        listenables;
    for (; i < (this.subscriptions || []).length; ++i) {
        listenables = [].concat(this.subscriptions[i].listenable);
        for (j = 0; j < listenables.length; j++) {
            listener = listenables[j];
            if (listener === listenable || listener.hasListener && listener.hasListener(listenable)) {
                return true;
            }
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.joinConcat"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinConcat ()](#apidoc.element.reflux.ListenerMethods.joinConcat)
- description and source-code
```javascript
joinConcat = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.joinLeading"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinLeading ()](#apidoc.element.reflux.ListenerMethods.joinLeading)
- description and source-code
```javascript
joinLeading = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.joinStrict"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinStrict ()](#apidoc.element.reflux.ListenerMethods.joinStrict)
- description and source-code
```javascript
joinStrict = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.joinTrailing"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>joinTrailing ()](#apidoc.element.reflux.ListenerMethods.joinTrailing)
- description and source-code
```javascript
joinTrailing = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.listenTo"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>listenTo (listenable, callback, defaultCallback)](#apidoc.element.reflux.ListenerMethods.listenTo)
- description and source-code
```javascript
function listenTo(listenable, callback, defaultCallback) {
    var desub,
        unsubscriber,
        subscriptionobj,
        subs = this.subscriptions = this.subscriptions || [];
    _.throwIf(this.validateListening(listenable));
    this.fetchInitialState(listenable, defaultCallback);
    desub = listenable.listen(this[callback] || callback, this);
    unsubscriber = function unsubscriber() {
        var index = subs.indexOf(subscriptionobj);
        _.throwIf(index === -1, "Tried to remove listen already gone from subscriptions list!");
        subs.splice(index, 1);
        desub();
    };
    subscriptionobj = {
        stop: unsubscriber,
        listenable: listenable
    };
    subs.push(subscriptionobj);
    return subscriptionobj;
}
```
- example usage
```shell
...
'''javascript
class StatusStore extends Reflux.Store
{
constructor()
{
    super();
    this.state = {flag:'OFFLINE'}; // <- set store's default state much like in React
    this.listenTo(statusUpdate, this.onStatusUpdate); // listen to the statusUpdate action
}

onStatusUpdate(status)
{
    var newFlag = status ? 'ONLINE' : 'OFFLINE';
    this.setState({flag:newFlag});
}
...
```

#### <a name="apidoc.element.reflux.ListenerMethods.listenToMany"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>listenToMany (listenables)](#apidoc.element.reflux.ListenerMethods.listenToMany)
- description and source-code
```javascript
function listenToMany(listenables) {
    var allListenables = flattenListenables(listenables);
    for (var key in allListenables) {
        var cbname = _.callbackName(key),
            localname = this[cbname] ? cbname : this[key] ? key : undefined;
        if (localname) {
            this.listenTo(allListenables[key], localname, this[cbname + "Default"] || this[localname + "Default"] || localname);
        }
    }
}
```
- example usage
```shell
...
						Combined[key] = obj[key];
					}
				});
			} else {
				Combined = v;
			}
			this.__listenables__ = Combined;
			this.listenToMany(Combined);
		},
		enumerable: true,
		configurable: true
	});
	
	// allows simple usage of 'this.setState(obj)' within the store to both update the state and trigger the store to update
	// components that it is attached to in a simple way that is idiomatic with React
...
```

#### <a name="apidoc.element.reflux.ListenerMethods.stopListeningTo"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>stopListeningTo (listenable)](#apidoc.element.reflux.ListenerMethods.stopListeningTo)
- description and source-code
```javascript
function stopListeningTo(listenable) {
    var sub,
        i = 0,
        subs = this.subscriptions || [];
    for (; i < subs.length; i++) {
        sub = subs[i];
        if (sub.listenable === listenable) {
            sub.stop();
            _.throwIf(subs.indexOf(sub) !== -1, "Failed to remove listen from subscriptions list!");
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.stopListeningToAll"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>stopListeningToAll ()](#apidoc.element.reflux.ListenerMethods.stopListeningToAll)
- description and source-code
```javascript
function stopListeningToAll() {
    var remaining,
        subs = this.subscriptions || [];
    while (remaining = subs.length) {
        subs[0].stop();
        _.throwIf(subs.length !== remaining - 1, "Failed to remove listen from subscriptions list!");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMethods.validateListening"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMethods.</span>validateListening (listenable)](#apidoc.element.reflux.ListenerMethods.validateListening)
- description and source-code
```javascript
function validateListening(listenable) {
    if (listenable === this) {
        return "Listener is not able to listen to itself";
    }
    if (!_.isFunction(listenable.listen)) {
        return listenable + " is missing a listen method";
    }
    if (listenable.hasListener && listenable.hasListener(this)) {
        return "Listener cannot listen to this listenable because of circular loop";
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.ListenerMixin"></a>[module reflux.ListenerMixin](#apidoc.module.reflux.ListenerMixin)

#### <a name="apidoc.element.reflux.ListenerMixin.componentWillUnmount"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>componentWillUnmount ()](#apidoc.element.reflux.ListenerMixin.componentWillUnmount)
- description and source-code
```javascript
function stopListeningToAll() {
    var remaining,
        subs = this.subscriptions || [];
    while (remaining = subs.length) {
        subs[0].stop();
        _.throwIf(subs.length !== remaining - 1, "Failed to remove listen from subscriptions list!");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.fetchInitialState"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>fetchInitialState (listenable, defaultCallback)](#apidoc.element.reflux.ListenerMixin.fetchInitialState)
- description and source-code
```javascript
function fetchInitialState(listenable, defaultCallback) {
    defaultCallback = defaultCallback && this[defaultCallback] || defaultCallback;
    var me = this;
    if (_.isFunction(defaultCallback) && _.isFunction(listenable.getInitialState)) {
        var data = listenable.getInitialState();
        if (data && _.isFunction(data.then)) {
            data.then(function () {
                defaultCallback.apply(me, arguments);
            });
        } else {
            defaultCallback.call(this, data);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.hasListener"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>hasListener (listenable)](#apidoc.element.reflux.ListenerMixin.hasListener)
- description and source-code
```javascript
function hasListener(listenable) {
    var i = 0,
        j,
        listener,
        listenables;
    for (; i < (this.subscriptions || []).length; ++i) {
        listenables = [].concat(this.subscriptions[i].listenable);
        for (j = 0; j < listenables.length; j++) {
            listener = listenables[j];
            if (listener === listenable || listener.hasListener && listener.hasListener(listenable)) {
                return true;
            }
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.joinConcat"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinConcat ()](#apidoc.element.reflux.ListenerMixin.joinConcat)
- description and source-code
```javascript
joinConcat = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.joinLeading"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinLeading ()](#apidoc.element.reflux.ListenerMixin.joinLeading)
- description and source-code
```javascript
joinLeading = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.joinStrict"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinStrict ()](#apidoc.element.reflux.ListenerMixin.joinStrict)
- description and source-code
```javascript
joinStrict = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.joinTrailing"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>joinTrailing ()](#apidoc.element.reflux.ListenerMixin.joinTrailing)
- description and source-code
```javascript
joinTrailing = function () /* listenables..., callback*/{
    _.throwIf(arguments.length < 2, "Cannot create a join with less than 2 listenables!");
    var listenables = slice.call(arguments),
        callback = listenables.pop(),
        numberOfListenables = listenables.length,
        join = {
        numberOfListenables: numberOfListenables,
        callback: this[callback] || callback,
        listener: this,
        strategy: strategy
    },
        i,
        cancels = [],
        subobj;
    for (i = 0; i < numberOfListenables; i++) {
        _.throwIf(this.validateListening(listenables[i]));
    }
    for (i = 0; i < numberOfListenables; i++) {
        cancels.push(listenables[i].listen(newListener(i, join), this));
    }
    reset(join);
    subobj = { listenable: listenables };
    subobj.stop = makeStopper(subobj, cancels, this);
    this.subscriptions = (this.subscriptions || []).concat(subobj);
    return subobj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.listenTo"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>listenTo (listenable, callback, defaultCallback)](#apidoc.element.reflux.ListenerMixin.listenTo)
- description and source-code
```javascript
function listenTo(listenable, callback, defaultCallback) {
    var desub,
        unsubscriber,
        subscriptionobj,
        subs = this.subscriptions = this.subscriptions || [];
    _.throwIf(this.validateListening(listenable));
    this.fetchInitialState(listenable, defaultCallback);
    desub = listenable.listen(this[callback] || callback, this);
    unsubscriber = function unsubscriber() {
        var index = subs.indexOf(subscriptionobj);
        _.throwIf(index === -1, "Tried to remove listen already gone from subscriptions list!");
        subs.splice(index, 1);
        desub();
    };
    subscriptionobj = {
        stop: unsubscriber,
        listenable: listenable
    };
    subs.push(subscriptionobj);
    return subscriptionobj;
}
```
- example usage
```shell
...
'''javascript
class StatusStore extends Reflux.Store
{
constructor()
{
    super();
    this.state = {flag:'OFFLINE'}; // <- set store's default state much like in React
    this.listenTo(statusUpdate, this.onStatusUpdate); // listen to the statusUpdate action
}

onStatusUpdate(status)
{
    var newFlag = status ? 'ONLINE' : 'OFFLINE';
    this.setState({flag:newFlag});
}
...
```

#### <a name="apidoc.element.reflux.ListenerMixin.listenToMany"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>listenToMany (listenables)](#apidoc.element.reflux.ListenerMixin.listenToMany)
- description and source-code
```javascript
function listenToMany(listenables) {
    var allListenables = flattenListenables(listenables);
    for (var key in allListenables) {
        var cbname = _.callbackName(key),
            localname = this[cbname] ? cbname : this[key] ? key : undefined;
        if (localname) {
            this.listenTo(allListenables[key], localname, this[cbname + "Default"] || this[localname + "Default"] || localname);
        }
    }
}
```
- example usage
```shell
...
						Combined[key] = obj[key];
					}
				});
			} else {
				Combined = v;
			}
			this.__listenables__ = Combined;
			this.listenToMany(Combined);
		},
		enumerable: true,
		configurable: true
	});
	
	// allows simple usage of 'this.setState(obj)' within the store to both update the state and trigger the store to update
	// components that it is attached to in a simple way that is idiomatic with React
...
```

#### <a name="apidoc.element.reflux.ListenerMixin.stopListeningTo"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>stopListeningTo (listenable)](#apidoc.element.reflux.ListenerMixin.stopListeningTo)
- description and source-code
```javascript
function stopListeningTo(listenable) {
    var sub,
        i = 0,
        subs = this.subscriptions || [];
    for (; i < subs.length; i++) {
        sub = subs[i];
        if (sub.listenable === listenable) {
            sub.stop();
            _.throwIf(subs.indexOf(sub) !== -1, "Failed to remove listen from subscriptions list!");
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.stopListeningToAll"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>stopListeningToAll ()](#apidoc.element.reflux.ListenerMixin.stopListeningToAll)
- description and source-code
```javascript
function stopListeningToAll() {
    var remaining,
        subs = this.subscriptions || [];
    while (remaining = subs.length) {
        subs[0].stop();
        _.throwIf(subs.length !== remaining - 1, "Failed to remove listen from subscriptions list!");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.ListenerMixin.validateListening"></a>[function <span class="apidocSignatureSpan">reflux.ListenerMixin.</span>validateListening (listenable)](#apidoc.element.reflux.ListenerMixin.validateListening)
- description and source-code
```javascript
function validateListening(listenable) {
    if (listenable === this) {
        return "Listener is not able to listen to itself";
    }
    if (!_.isFunction(listenable.listen)) {
        return listenable + " is missing a listen method";
    }
    if (listenable.hasListener && listenable.hasListener(this)) {
        return "Listener cannot listen to this listenable because of circular loop";
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.PublisherMethods"></a>[module reflux.PublisherMethods](#apidoc.module.reflux.PublisherMethods)

#### <a name="apidoc.element.reflux.PublisherMethods.deferWith"></a>[function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>deferWith (callback)](#apidoc.element.reflux.PublisherMethods.deferWith)
- description and source-code
```javascript
function deferWith(callback) {
    var oldTrigger = this.trigger,
        ctx = this,
        resolver = function resolver() {
        oldTrigger.apply(ctx, arguments);
    };
    this.trigger = function () {
        callback.apply(ctx, [resolver].concat([].splice.call(arguments, 0)));
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PublisherMethods.listen"></a>[function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>listen (callback, bindContext)](#apidoc.element.reflux.PublisherMethods.listen)
- description and source-code
```javascript
function listen(callback, bindContext) {
    bindContext = bindContext || this;
    var eventHandler = function eventHandler(args) {
        if (aborted) {
            return;
        }
        callback.apply(bindContext, args);
    },
        me = this,
        aborted = false;
    this.emitter.addListener(this.eventLabel, eventHandler);
    return function () {
        aborted = true;
        me.emitter.removeListener(me.eventLabel, eventHandler);
    };
}
```
- example usage
```shell
...
					} else if (storeId) {
						Reflux.GlobalState[storeId] = str.state;
					}
					// if no id, then no messing with global state
				}
				// listen/subscribe for the ".trigger()" in the store, and track the unsubscribes so that we can unsubscribe on unmount
				if (!Reflux.serverMode) {
					this.__storeunsubscribes__.push(str.listen(onStoreTrigger));
				}
				// run set state so that it mixes in the props from the store with the component
				var updateObj = filterByStoreKeys(this.storeKeys, str.state);
				if (updateObj) {
					this.setState(updateObj);
				}
			}
...
```

#### <a name="apidoc.element.reflux.PublisherMethods.preEmit"></a>[function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>preEmit ()](#apidoc.element.reflux.PublisherMethods.preEmit)
- description and source-code
```javascript
function preEmit() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PublisherMethods.shouldEmit"></a>[function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>shouldEmit ()](#apidoc.element.reflux.PublisherMethods.shouldEmit)
- description and source-code
```javascript
function shouldEmit() {
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PublisherMethods.trigger"></a>[function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>trigger ()](#apidoc.element.reflux.PublisherMethods.trigger)
- description and source-code
```javascript
function trigger() {
    var args = arguments,
        pre = this.preEmit.apply(this, args);
    args = pre === undefined ? args : _.isArguments(pre) ? pre : [].concat(pre);
    if (this.shouldEmit.apply(this, args)) {
        this.emitter.emit(this.eventLabel, args);
    }
}
```
- example usage
```shell
...
						Reflux.GlobalState[storeId] = str.state;
					// otherwise (if it has an id) set the global state to the default state of the store
					} else if (storeId) {
						Reflux.GlobalState[storeId] = str.state;
					}
					// if no id, then no messing with global state
				}
				// listen/subscribe for the ".trigger()" in the store, and track the unsubscribes so that we can unsubscribe on unmount
				if (!Reflux.serverMode) {
					this.__storeunsubscribes__.push(str.listen(onStoreTrigger));
				}
				// run set state so that it mixes in the props from the store with the component
				var updateObj = filterByStoreKeys(this.storeKeys, str.state);
				if (updateObj) {
					this.setState(updateObj);
...
```

#### <a name="apidoc.element.reflux.PublisherMethods.triggerAsync"></a>[function <span class="apidocSignatureSpan">reflux.PublisherMethods.</span>triggerAsync ()](#apidoc.element.reflux.PublisherMethods.triggerAsync)
- description and source-code
```javascript
function triggerAsync() {
    var args = arguments,
        me = this;
    _.nextTick(function () {
        me.trigger.apply(me, args);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.PureComponent"></a>[module reflux.PureComponent](#apidoc.module.reflux.PureComponent)

#### <a name="apidoc.element.reflux.PureComponent.PureComponent"></a>[function <span class="apidocSignatureSpan">reflux.</span>PureComponent (props, context, updater)](#apidoc.element.reflux.PureComponent.PureComponent)
- description and source-code
```javascript
PureComponent = function (props, context, updater) {
		_extend.call(this, props, context, updater);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PureComponent.extend"></a>[function <span class="apidocSignatureSpan">reflux.PureComponent.</span>extend (clss)](#apidoc.element.reflux.PureComponent.extend)
- description and source-code
```javascript
extend = function (clss) {
		return defineReact(null, null, clss);
	}
```
- example usage
```shell
...
        }

        return _.object([key],[listenable.getInitialState()]);
    },
    componentDidMount: function() {
        var me = this;

        _.extend(me, ListenerMethods);

        this.listenTo(listenable, function(v) {
            me.setState(_.object([key],[v]));
        });
    },
    componentWillUnmount: ListenerMixin.componentWillUnmount
};
...
```



# <a name="apidoc.module.reflux.PureComponent.prototype"></a>[module reflux.PureComponent.prototype](#apidoc.module.reflux.PureComponent.prototype)

#### <a name="apidoc.element.reflux.PureComponent.prototype.componentWillMount"></a>[function <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>componentWillMount ()](#apidoc.element.reflux.PureComponent.prototype.componentWillMount)
- description and source-code
```javascript
componentWillMount = function () {
		// if there is a this.store then simply push it onto the this.stores array or make one if needed
		if (this.store) {
			if (Array.isArray(this.stores)) {
				this.stores.unshift(this.store);
			} else {
				this.stores = [this.store];
			}
		}
		
		if (this.stores) {
			this.__storeunsubscribes__ = this.__storeunsubscribes__ || [];
			var sS = this.setState.bind(this);
			// this handles the triggering of a store, checking what's updated if proto.storeKeys is utilized
			var onStoreTrigger = function(obj){
				var updateObj = filterByStoreKeys(this.storeKeys, obj);
				if (updateObj) {
					sS(updateObj);
				}
			}.bind(this);
			// for each store in this.stores...
			for (var i = 0, ii = this.stores.length; i < ii; i++) {
				var str = this.stores[i];
				// if's a function then we know it's a class getting passed, not an instance
				if (typeof str === 'function') {
					var storeId = str.id;
					// if there is NOT a .singleton property on the store then this store has not been initialized yet, so do so
					if (!str.singleton) {
						str.singleton = new str();
						if (storeId) {
							Reflux.stores[storeId] = str.singleton;
						}
					}
					// before we weren't sure if we were working with an instance or class, so now we know an instance is created set it
					// to the variables we were using so that we can just continue on knowing it's the instance we're working with
					this.stores[i] = str = str.singleton;
					// the instance should have an .id property as well if the class does, so set that here
					str.id = storeId;
					// if there is an id and there is a global state property for this store then merge
					// the properties from that global state into the default state of the store AND then
					// set the global state to that new state (since it may have previously been partial)
					if (storeId && Reflux.GlobalState[storeId]) {
						for (var key in Reflux.GlobalState[storeId]) {
							str.state[key] = Reflux.GlobalState[storeId][key];
						}
						Reflux.GlobalState[storeId] = str.state;
					// otherwise (if it has an id) set the global state to the default state of the store
					} else if (storeId) {
						Reflux.GlobalState[storeId] = str.state;
					}
					// if no id, then no messing with global state
				}
				// listen/subscribe for the ".trigger()" in the store, and track the unsubscribes so that we can unsubscribe on unmount
				if (!Reflux.serverMode) {
					this.__storeunsubscribes__.push(str.listen(onStoreTrigger));
				}
				// run set state so that it mixes in the props from the store with the component
				var updateObj = filterByStoreKeys(this.storeKeys, str.state);
				if (updateObj) {
					this.setState(updateObj);
				}
			}
		}
		
		// mapStoreToState needs to know if is ready to map or must wait
		this.__readytomap__ = true;
		// if there are mappings that were delayed, do them now
		var dmaps = this.__delayedmaps__;
		if (dmaps) {
			for (var j=0,jj=dmaps.length; j<jj; j++) {
				dmaps[j].func( dmaps[j].state );
			}
		}
		this.__delayedmaps__ = null;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PureComponent.prototype.componentWillUnmount"></a>[function <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>componentWillUnmount ()](#apidoc.element.reflux.PureComponent.prototype.componentWillUnmount)
- description and source-code
```javascript
componentWillUnmount = function () {
		if (this.__storeunsubscribes__) {
			for (var i = 0, ii = this.__storeunsubscribes__.length; i < ii; i++) {
				this.__storeunsubscribes__[i]();
			}
		}
		this.__readytomap__ = false;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.PureComponent.prototype.mapStoreToState"></a>[function <span class="apidocSignatureSpan">reflux.PureComponent.prototype.</span>mapStoreToState (store, filterFunc)](#apidoc.element.reflux.PureComponent.prototype.mapStoreToState)
- description and source-code
```javascript
mapStoreToState = function (store, filterFunc)
	{
		// make sure we have a proper singleton instance to work with
		if (typeof store === 'function') {
			if (store.singleton) {
				store = store.singleton;
			} else {
				store = Reflux.initStore(store);
			}
		}
		
		// we need a closure so that the called function can remember the proper filter function to use, so function gets defined here
		var self = this;
		function onMapStoreTrigger(obj) {
			// get an object
			var update = filterFunc.call(self, obj);
			// if no object returned from filter functions do nothing
			if (!update) {
				return;
			}
			// check if the update actually has any mapped props
			/*jshint unused: false */
			var hasProps = false;
			for (var check in update) {
				hasProps = true;
				break;
			}
			// if there were props mapped, then update via setState
			if (hasProps) {
				self.setState(update);
			}
		}
		
		// add the listener to know when the store is triggered
		this.__storeunsubscribes__ = this.__storeunsubscribes__ || [];
		this.__storeunsubscribes__.push(store.listen(onMapStoreTrigger));
		
		// now actually run onMapStoreTrigger with the full store state so that we immediately have all store state mapped to component
 state
		if (this.__readytomap__) {
			onMapStoreTrigger(store.state);
		} else {
			this.__delayedmaps__ = this.__delayedmaps__ || [];
			this.__delayedmaps__.push({func:onMapStoreTrigger, state:store.state});
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.Store"></a>[module reflux.Store](#apidoc.module.reflux.Store)

#### <a name="apidoc.element.reflux.Store.Store"></a>[function <span class="apidocSignatureSpan">reflux.</span>Store ()](#apidoc.element.reflux.Store.Store)
- description and source-code
```javascript
Store = function () {
		// extending doesn't really work well here, so instead we create an internal instance
		// and just loop through its properties/methods and make a getter/setter for each
		// that will actually be getting and setting on that internal instance.
		this.__store__ = Reflux.createStore();
		this.state = {};
		var self = this;
		for (var key in this.__store__) {
			/*jshint loopfunc: true */
			(function (prop) {
				Object.defineProperty(self, prop, {
					get: function () { return self.__store__[prop]; },
					set: function (v) { self.__store__[prop] = v; }
				});
			})(key);
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.Store.prototype"></a>[module reflux.Store.prototype](#apidoc.module.reflux.Store.prototype)

#### <a name="apidoc.element.reflux.Store.prototype.setState"></a>[function <span class="apidocSignatureSpan">reflux.Store.prototype.</span>setState (obj)](#apidoc.element.reflux.Store.prototype.setState)
- description and source-code
```javascript
setState = function (obj) {
		// Object.assign(this.state, obj); // later turn this to Object.assign and remove loop once support is good enough
		for (var key in obj) {
			this.state[key] = obj[key];
		}
		// if there's an id (i.e. it's being tracked by the global state) then make sure to update the global state
		if (this.id) {
			Reflux.GlobalState[this.id] = this.state;
		}
		// trigger, because any component it's attached to is listening and will merge the store state into its own on a store trigger
		this.trigger(obj);
	}
```
- example usage
```shell
...
        this.state = {flag:'OFFLINE'}; // <- set store's default state much like in React
        this.listenTo(statusUpdate, this.onStatusUpdate); // listen to the statusUpdate action
    }

    onStatusUpdate(status)
    {
        var newFlag = status ? 'ONLINE' : 'OFFLINE';
        this.setState({flag:newFlag});
    }
}
'''

In the above example, whenever the action 'statusUpdate' is called, the store's 'onStatusUpdate' callback will be called with whatever
 parameters were sent in the action. E.g. if the action is called as 'statusUpdate(true)' then the 'status' argument in the 'onStatusUpdate
' function is 'true'.

Stores also integrate easily with sets of actions via things like 'this.listenables'. When an actions object (or an Array of multiple
 actions objects) is applied to 'this.listenables' you may automatically add listeners simply by naming convention. Just name the
 functions either after the action name (such as 'actionName', or the camelcased action name preceded with "on", (such as 'onActionName
').
...
```



# <a name="apidoc.module.reflux.__keep"></a>[module reflux.__keep](#apidoc.module.reflux.__keep)

#### <a name="apidoc.element.reflux.__keep.addAction"></a>[function <span class="apidocSignatureSpan">reflux.__keep.</span>addAction (act)](#apidoc.element.reflux.__keep.addAction)
- description and source-code
```javascript
function addAction(act) {
	if (use) {
		createdActions.push(act);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.__keep.addStore"></a>[function <span class="apidocSignatureSpan">reflux.__keep.</span>addStore (str)](#apidoc.element.reflux.__keep.addStore)
- description and source-code
```javascript
function addStore(str) {
	if (use) {
		createdStores.push(str);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.__keep.reset"></a>[function <span class="apidocSignatureSpan">reflux.__keep.</span>reset ()](#apidoc.element.reflux.__keep.reset)
- description and source-code
```javascript
function reset() {
	while (createdStores.length) {
		createdStores.pop();
	}
	while (createdActions.length) {
		createdActions.pop();
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.__keep.useKeep"></a>[function <span class="apidocSignatureSpan">reflux.__keep.</span>useKeep ()](#apidoc.element.reflux.__keep.useKeep)
- description and source-code
```javascript
function useKeep() {
	var bool = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : true;

	use = bool;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.utils"></a>[module reflux.utils](#apidoc.module.reflux.utils)

#### <a name="apidoc.element.reflux.utils.EventEmitter"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>EventEmitter ()](#apidoc.element.reflux.utils.EventEmitter)
- description and source-code
```javascript
function EventEmitter() { /* Nothing to set */ }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.callbackName"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>callbackName (string, prefix)](#apidoc.element.reflux.utils.callbackName)
- description and source-code
```javascript
function callbackName(string, prefix) {
    prefix = prefix || "on";
    return prefix + exports.capitalize(string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.capitalize"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>capitalize (string)](#apidoc.element.reflux.utils.capitalize)
- description and source-code
```javascript
function capitalize(string) {
    return string.charAt(0).toUpperCase() + string.slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.extend"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>extend (obj)](#apidoc.element.reflux.utils.extend)
- description and source-code
```javascript
function extend(obj) {
    if (!isObject(obj)) {
        return obj;
    }
    var source, keys, prop;
    for (var i = 1, length = arguments.length; i < length; i++) {
        source = arguments[i];
        keys = Object.keys(source);
        for (var j = 0; j < keys.length; j++) {
            prop = keys[j];
            if (Object.getOwnPropertyDescriptor && Object.defineProperty) {
                var propertyDescriptor = Object.getOwnPropertyDescriptor(source, prop);
                Object.defineProperty(obj, prop, propertyDescriptor);
            } else {
                obj[prop] = source[prop];
            }
        }
    }
    return obj;
}
```
- example usage
```shell
...
        }

        return _.object([key],[listenable.getInitialState()]);
    },
    componentDidMount: function() {
        var me = this;

        _.extend(me, ListenerMethods);

        this.listenTo(listenable, function(v) {
            me.setState(_.object([key],[v]));
        });
    },
    componentWillUnmount: ListenerMixin.componentWillUnmount
};
...
```

#### <a name="apidoc.element.reflux.utils.inherits"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>inherits (subClass, superClass)](#apidoc.element.reflux.utils.inherits)
- description and source-code
```javascript
inherits = function (subClass, superClass) {
	if (typeof superClass !== "function" && superClass !== null) {
		throw new TypeError("Super expression must either be null or a function, not " + typeof superClass);
	}
	subClass.prototype = Object.create(superClass && superClass.prototype, {
		constructor: {
			value: subClass,
			enumerable: false,
			writable: true,
			configurable: true
		}
	});
	if (superClass) {
		if (Object.setPrototypeOf) {
			Object.setPrototypeOf(subClass, superClass);
		} else {
			/* jshint proto: true */
			subClass.__proto__ = superClass;
		}
	}
}
```
- example usage
```shell
...
	 * in the trigger into the component automatically.
	 */
	var RefluxComponent = function(props, context, updater) {
		_extend.call(this, props, context, updater);
	};
	
	// equivalent of 'extends React.Component' or other class if provided via 'extend' param
	Reflux.utils.inherits(RefluxComponent, _extend);
	
	proto = RefluxComponent.prototype;
	
	/**
	 * this.storeKeys
	 * When this is a falsey value (null by default) the component mixes in
	 * all properties from the stores attached to it and updates on changes
...
```

#### <a name="apidoc.element.reflux.utils.isArguments"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>isArguments (value)](#apidoc.element.reflux.utils.isArguments)
- description and source-code
```javascript
function isArguments(value) {
    return (typeof value === "undefined" ? "undefined" : _typeof(value)) === "object" && "callee" in value && typeof value.length
 === "number";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.isFunction"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>isFunction (value)](#apidoc.element.reflux.utils.isFunction)
- description and source-code
```javascript
function isFunction(value) {
    return typeof value === "function";
}
```
- example usage
```shell
...

module.exports = function(listenable, key) {

    _.throwIf(typeof(key) === 'undefined', 'Reflux.connect() requires a key.');

    return {
getInitialState: function() {
    if (!_.isFunction(listenable.getInitialState)) {
        return {};
    }

    return _.object([key],[listenable.getInitialState()]);
},
componentDidMount: function() {
    var me = this;
...
```

#### <a name="apidoc.element.reflux.utils.isObject"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>isObject (obj)](#apidoc.element.reflux.utils.isObject)
- description and source-code
```javascript
function isObject(obj) {
    var type = typeof obj === "undefined" ? "undefined" : _typeof(obj);
    return type === "function" || type === "object" && !!obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.nextTick"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>nextTick (callback)](#apidoc.element.reflux.utils.nextTick)
- description and source-code
```javascript
function nextTick(callback) {
    setTimeout(callback, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.object"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>object (keys, vals)](#apidoc.element.reflux.utils.object)
- description and source-code
```javascript
function object(keys, vals) {
    var o = {},
        i = 0;
    for (; i < keys.length; i++) {
        o[keys[i]] = vals[i];
    }
    return o;
}
```
- example usage
```shell
...

    return {
        getInitialState: function() {
if (!_.isFunction(listenable.getInitialState)) {
    return {};
}

return _.object([key],[listenable.getInitialState()]);
        },
        componentDidMount: function() {
var me = this;

_.extend(me, ListenerMethods);

this.listenTo(listenable, function(v) {
...
```

#### <a name="apidoc.element.reflux.utils.throwIf"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>throwIf (val, msg)](#apidoc.element.reflux.utils.throwIf)
- description and source-code
```javascript
function throwIf(val, msg) {
    if (val) {
        throw Error(msg || val);
    }
}
```
- example usage
```shell
...

var ListenerMethods = require('reflux-core/lib/ListenerMethods'),
ListenerMixin = require('./ListenerMixin'),
_ = require('reflux-core/lib/utils');

module.exports = function(listenable, key) {

_.throwIf(typeof(key) === 'undefined', 'Reflux.connect() requires a key.');

return {
    getInitialState: function() {
        if (!_.isFunction(listenable.getInitialState)) {
            return {};
        }
...
```



# <a name="apidoc.module.reflux.utils.EventEmitter"></a>[module reflux.utils.EventEmitter](#apidoc.module.reflux.utils.EventEmitter)

#### <a name="apidoc.element.reflux.utils.EventEmitter.EventEmitter"></a>[function <span class="apidocSignatureSpan">reflux.utils.</span>EventEmitter ()](#apidoc.element.reflux.utils.EventEmitter.EventEmitter)
- description and source-code
```javascript
function EventEmitter() { /* Nothing to set */ }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.reflux.utils.EventEmitter.prototype"></a>[module reflux.utils.EventEmitter.prototype](#apidoc.module.reflux.utils.EventEmitter.prototype)

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.addListener"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>addListener (event, fn, context)](#apidoc.element.reflux.utils.EventEmitter.prototype.addListener)
- description and source-code
```javascript
function on(event, fn, context) {
  var listener = new EE(fn, context || this)
    , evt = prefix ? prefix + event : event;

  if (!this._events) this._events = prefix ? {} : Object.create(null);
  if (!this._events[evt]) this._events[evt] = listener;
  else {
    if (!this._events[evt].fn) this._events[evt].push(listener);
    else this._events[evt] = [
      this._events[evt], listener
    ];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.emit"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>emit (event, a1, a2, a3, a4, a5)](#apidoc.element.reflux.utils.EventEmitter.prototype.emit)
- description and source-code
```javascript
function emit(event, a1, a2, a3, a4, a5) {
  var evt = prefix ? prefix + event : event;

  if (!this._events || !this._events[evt]) return false;

  var listeners = this._events[evt]
    , len = arguments.length
    , args
    , i;

  if ('function' === typeof listeners.fn) {
    if (listeners.once) this.removeListener(event, listeners.fn, undefined, true);

    switch (len) {
      case 1: return listeners.fn.call(listeners.context), true;
      case 2: return listeners.fn.call(listeners.context, a1), true;
      case 3: return listeners.fn.call(listeners.context, a1, a2), true;
      case 4: return listeners.fn.call(listeners.context, a1, a2, a3), true;
      case 5: return listeners.fn.call(listeners.context, a1, a2, a3, a4), true;
      case 6: return listeners.fn.call(listeners.context, a1, a2, a3, a4, a5), true;
    }

    for (i = 1, args = new Array(len -1); i < len; i++) {
      args[i - 1] = arguments[i];
    }

    listeners.fn.apply(listeners.context, args);
  } else {
    var length = listeners.length
      , j;

    for (i = 0; i < length; i++) {
      if (listeners[i].once) this.removeListener(event, listeners[i].fn, undefined, true);

      switch (len) {
        case 1: listeners[i].fn.call(listeners[i].context); break;
        case 2: listeners[i].fn.call(listeners[i].context, a1); break;
        case 3: listeners[i].fn.call(listeners[i].context, a1, a2); break;
        default:
          if (!args) for (j = 1, args = new Array(len -1); j < len; j++) {
            args[j - 1] = arguments[j];
          }

          listeners[i].fn.apply(listeners[i].context, args);
      }
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>eventNames ()](#apidoc.element.reflux.utils.EventEmitter.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  var events = this._events
    , names = []
    , name;

  if (!events) return names;

  for (name in events) {
    if (has.call(events, name)) names.push(prefix ? name.slice(1) : name);
  }

  if (Object.getOwnPropertySymbols) {
    return names.concat(Object.getOwnPropertySymbols(events));
  }

  return names;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.listeners"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>listeners (event, exists)](#apidoc.element.reflux.utils.EventEmitter.prototype.listeners)
- description and source-code
```javascript
function listeners(event, exists) {
  var evt = prefix ? prefix + event : event
    , available = this._events && this._events[evt];

  if (exists) return !!available;
  if (!available) return [];
  if (available.fn) return [available.fn];

  for (var i = 0, l = available.length, ee = new Array(l); i < l; i++) {
    ee[i] = available[i].fn;
  }

  return ee;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.off"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>off (event, fn, context, once)](#apidoc.element.reflux.utils.EventEmitter.prototype.off)
- description and source-code
```javascript
function removeListener(event, fn, context, once) {
  var evt = prefix ? prefix + event : event;

  if (!this._events || !this._events[evt]) return this;

  var listeners = this._events[evt]
    , events = [];

  if (fn) {
    if (listeners.fn) {
      if (
           listeners.fn !== fn
        || (once && !listeners.once)
        || (context && listeners.context !== context)
      ) {
        events.push(listeners);
      }
    } else {
      for (var i = 0, length = listeners.length; i < length; i++) {
        if (
             listeners[i].fn !== fn
          || (once && !listeners[i].once)
          || (context && listeners[i].context !== context)
        ) {
          events.push(listeners[i]);
        }
      }
    }
  }

  //
  // Reset the array, or remove it completely if we have no more listeners.
  //
  if (events.length) {
    this._events[evt] = events.length === 1 ? events[0] : events;
  } else {
    delete this._events[evt];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.on"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>on (event, fn, context)](#apidoc.element.reflux.utils.EventEmitter.prototype.on)
- description and source-code
```javascript
function on(event, fn, context) {
  var listener = new EE(fn, context || this)
    , evt = prefix ? prefix + event : event;

  if (!this._events) this._events = prefix ? {} : Object.create(null);
  if (!this._events[evt]) this._events[evt] = listener;
  else {
    if (!this._events[evt].fn) this._events[evt].push(listener);
    else this._events[evt] = [
      this._events[evt], listener
    ];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.once"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>once (event, fn, context)](#apidoc.element.reflux.utils.EventEmitter.prototype.once)
- description and source-code
```javascript
function once(event, fn, context) {
  var listener = new EE(fn, context || this, true)
    , evt = prefix ? prefix + event : event;

  if (!this._events) this._events = prefix ? {} : Object.create(null);
  if (!this._events[evt]) this._events[evt] = listener;
  else {
    if (!this._events[evt].fn) this._events[evt].push(listener);
    else this._events[evt] = [
      this._events[evt], listener
    ];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>removeAllListeners (event)](#apidoc.element.reflux.utils.EventEmitter.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(event) {
  if (!this._events) return this;

  if (event) delete this._events[prefix ? prefix + event : event];
  else this._events = prefix ? {} : Object.create(null);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>removeListener (event, fn, context, once)](#apidoc.element.reflux.utils.EventEmitter.prototype.removeListener)
- description and source-code
```javascript
function removeListener(event, fn, context, once) {
  var evt = prefix ? prefix + event : event;

  if (!this._events || !this._events[evt]) return this;

  var listeners = this._events[evt]
    , events = [];

  if (fn) {
    if (listeners.fn) {
      if (
           listeners.fn !== fn
        || (once && !listeners.once)
        || (context && listeners.context !== context)
      ) {
        events.push(listeners);
      }
    } else {
      for (var i = 0, length = listeners.length; i < length; i++) {
        if (
             listeners[i].fn !== fn
          || (once && !listeners[i].once)
          || (context && listeners[i].context !== context)
        ) {
          events.push(listeners[i]);
        }
      }
    }
  }

  //
  // Reset the array, or remove it completely if we have no more listeners.
  //
  if (events.length) {
    this._events[evt] = events.length === 1 ? events[0] : events;
  } else {
    delete this._events[evt];
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.reflux.utils.EventEmitter.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">reflux.utils.EventEmitter.prototype.</span>setMaxListeners ()](#apidoc.element.reflux.utils.EventEmitter.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners() {
  return this;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
