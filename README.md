# svelte-d3-rollup
A basic responsive application built with rollup, implementing two simple d3 components in svelte.

### published to github pages here

`https://jklemke.github.io/svelte-d3-rollup/` The index.html simply includes the compiled bundle.js.


### npm commands to build and run

`npm run build` compiles /src/main.js and dependencies and places output in /public/build/bundle.js 

`npm run dev` compiles /src/main.js and dependencies and places output in /public/build/bundle.js, then recompiles when a source file change is saved

`npm run sirv` runs the sirv web server at localhost:5000/index.html and reloads the browser app automatically when new compiled code appears in /public


