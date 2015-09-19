# firstTsNgApp
This is for test purpose

Prerequisites:
- install node
- install typescript: npm install -g typescript
- install tsd package manager: npm install -g tsd
- install a node static server (for this project specific): npm install -g live-server

To be able to run the application:
- mkdir <dir> & cd <dir>
- git checkout https://github.com/capoli/firstTsNgApp.git
- npm install
- cd src
- tsd install
*** if tsd.json is missing execute form the src folder following command:
*** - tsd install angular2 es6-promise rx rx-lite --save

tsconfig schema: http://json.schemastore.org/tsconfig

To compile Typescript to Javascript execute from the root of the application folder:
- tsc -p src -w
*** this is to generate a .js file (and a .map.js file, helps debugger to navigate between js and ts) from a .ts file
*** with -w it will automatically watch for changes and recompile

To run the application execute from the root of the application folder:
live-server --open=src