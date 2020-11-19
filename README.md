# svelte-d3-rollup
A basic responsive application built with rollup, implementing two simple d3 components in svelte.

### published to github pages here
The index.html just has to include the compiled bundle.js

https://jklemke.github.io/svelte-d3-rollup/ 

### npm commands to build and run

`npm run build` compiles /src/main.js and dependencies and places output in /public/build/bundle.js 

`npm run dev` compiles /src/main.js and dependencies and places output in /public/build/bundle.js, then recompiles when a source file change is saved

`npm run sirv` runs the sirv web server at localhost:5000/index.html and reloads the browser app automatically when new compiled code appears in /public


