To run:

    yarn; yarn start

or

    npm install; npm start

### Expected:

- Parcel bundles the project, serves it at `localhost:1234`
- When you open it in a browser, it prints "it works" and the contents of `nanocomponent`.

### Actual:

Parcel hangs:

    $ yarn start
    yarn run v1.6.0
    (node:5033) [DEP0005] DeprecationWarning: Buffer() is deprecated due to security and usability issues. Please use the Buffer.alloc(), Buffer.allocUnsafe(), or Buffer.from() methods instead.
    $ parcel --no-cache index.html
    Server running at http://localhost:1234 
    ⏳  Building events.js...

### Environment:

|name|version|
|-|-|
|parcel-bundler|1.9.3|
|node|10.5.0|
|macOS|10.12.6|