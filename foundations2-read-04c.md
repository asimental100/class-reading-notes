Computers are asynchronous by design.

JavaScript is synchronous by default and is single threaded. This means that code cannot create new threads and run in parallel.

A promise is commonly defined as a proxy for a value that will eventually become available. Promises are one way to deal with asynchronous code, without writing too many callbacks in your code.

If you need to synchronize different promises, Promise.all() helps you define a list of promises, and execute something when they are all resolved.

Promise.race() runs as soon as one of the promises you pass to it resolves, and it runs the attached callback just once with the result of the first promise resolved.

Promises are a comparatively new feature of the JavaScript language that allow you to defer further actions until after a previous action has completed, or respond to its failure. This is useful for setting up a sequence of async operations to work correctly. This article shows you how promises work, how you'll see them in use with web APIs, and how to write your own.

Gretchen. Stop trying to make fetch happen. It's not going to happen.

fetch uses promises.
