# Assemblyscript Demo

This demo was built from following this [article](https://medium.com/@BenedekGagyi/the-simplest-way-to-get-started-with-webassembly-1f92f6f90d24), which shows how easy it is to use WebAssembly on a browser.

Using Assemblyscript we compile Typescript to WebAssembly, which can then be used on the browser.

In this example, we write a function that returns us a Fibonacci number for an integer. Check out [fib.ts](/src/fib.ts)

Then we run the command from our package.json to compile it

```bash
npm run compile

# OR

asc src/fib.ts -o dist/fib.wasm
```

We get a WebAssembly file, [fib.wasm](/dist/fib.wasm), that we can later load in our browser and use it with Javascript, [index.html](/dist/index.html).

Check out the live demo at [https://assemblyscript-demo.netlify.com](https://assemblyscript-demo.netlify.com)
