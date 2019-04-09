Jest TypeScript Web-Compatible Resolver
=======================================

TypeScript allows importing other TypeScript files with a `.js` extension, for
compatibility with the ES6 modules loader specification. Unfortunately, Jest
gets confused by this and complains that it's not able to find the JavaScript
file.

This is a resolver that catches that error, and then tries to resolve it again
but with a `.ts` extension.


Installation & Set-Up
---------------------

Install this module into your project using npm:

```
npm install -D jest-ts-webcompat-resolver
```

Then add it to your Jest config file as the resolver:

```
"resolver": "jest-ts-webcompat-resolver"
```


Licence
-------

This project is licensed under the [MIT Licence][mit].

[mit]:
  https://github.com/AyogoHealth/jest-ts-webcompat-resolver/blob/master/LICENSE
