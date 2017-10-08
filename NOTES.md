# SETTING UP ES6: NOTES FROM READING THE BOOK #

### October 6th 2017 ###
- Reading what Babel is, why it's important to ES6, how to set it up.
- Babel is a "next gen" compiler for JS.
- It is also known as a transpiler (source-to-source compiler), which means I and others can use ES6, but it will "transpile" to ES5 so the code can be used in older browsers that don't fully support ES6 yet.
- Babel has its own CLI to easily compile files.
- You compile the files with `$ babel filename.js`

### October 7th 2017 ###
- REPL basicly means a command line or CLI.
- Babel brings ES6 support to the Node.js REPL via `babel-node`.
- For transpilation you need 3 things: a transpiler (for your code), a package manager and a module system (for the complete app).
- I picked Microsoft Typescript as my transpiler.
- Transpilation can be done statically (before you deploy) or dynamically (which happens at runtime).
- With Typescript you can invoke module formats directly or with gulp, grunt etc. Module formats are: AMD, CommonJS, ES6 module loader
- In browsers, you transpile dynamically via a library plus a custom `<script type="...">` which is available with Babel.
- Going to be giving webpack, as a module system, a try.
- Linters and checkers analyze source code statically and report problems related to style, typing, etc. Apparently the best and most popular is ESLint.
- When the web app starts, feature detection is used to check whether ES6 is fully supported. If it is, the ES6 version of the app is used. Otherwise, the ES5 version is used.
- ES6 provides better features for classes and modules.
- `for-of` loop is used to iterate through iterable objects such as Arrays, Map, Set, String, TypedArray.

### October 8th 2017 ###
- Three types of features exist in ES6. Better syntax for existing features, new functionality in the standard library and completely new features.
- ES6 provides better features for *classes* and *modules*.
- The standard ES6 library now features *new methods for strings and arrays*, *promises* and *maps, sets*.
- Some features can never be transpiled to ES5 such as `let` and `const`, *symbols*, *generators* and *WeakMaps*.
- Dependencies are the packages used by the current package. They are installed into `node-modules` by `npm install`.
- A source map is a file that accompanies the transpilation output and maps the lines of the output to lines in the input files.