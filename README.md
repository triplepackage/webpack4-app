# Baltimore County Rental UI with ReactJs, Redux and Webpack 4

http://ec2-34-204-247-182.compute-1.amazonaws.com/

<pre>
Johns-MBP:GitHub admin$ mkdir webpack-app
Johns-MBP:GitHub admin$ cd webpack-app/
Johns-MBP:webpack-app admin$ mkdir -p src
Johns-MBP:webpack-app admin$ npm init -y
Wrote to /Users/admin/GitHub/webpack-app/package.json:

{
  "name": "webpack-app",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}


Johns-MBP:webpack-app admin$ npm i webpack --save-dev

> fsevents@1.2.4 install /Users/admin/GitHub/webpack-app/node_modules/fsevents
> node install

[fsevents] Success: "/Users/admin/GitHub/webpack-app/node_modules/fsevents/lib/binding/Release/node-v64-darwin-x64/fse.node" already installed
Pass --update-binary to reinstall or --build-from-source to recompile
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN webpack-app@1.0.0 No description
npm WARN webpack-app@1.0.0 No repository field.

+ webpack@4.25.0
added 383 packages from 298 contributors and audited 4147 packages in 11.944s
found 0 vulnerabilities

Johns-MBP:webpack-app admin$ npm i webpack-cli --save-dev
npm WARN webpack-app@1.0.0 No description
npm WARN webpack-app@1.0.0 No repository field.

+ webpack-cli@3.1.2
added 70 packages from 15 contributors and audited 4258 packages in 4.101s
found 0 vulnerabilities

Johns-MBP:webpack-app admin$ npm i @babel/core babel-loader @babel/preset-env @babel/preset-react --save-dev
npm WARN webpack-app@1.0.0 No description
npm WARN webpack-app@1.0.0 No repository field.

+ @babel/preset-react@7.0.0
+ babel-loader@8.0.4
+ @babel/core@7.1.2
+ @babel/preset-env@7.1.0
added 119 packages from 36 contributors and audited 5662 packages in 6.515s
found 0 vulnerabilities

Johns-MBP:webpack-app admin$ npm run build

> webpack-app@1.0.0 build /Users/admin/GitHub/webpack-app
> webpack --mode production

Hash: 1359004f743aa71104e6
Version: webpack 4.25.0
Time: 511ms
Built at: 11/05/2018 7:22:11 AM
  Asset       Size  Chunks             Chunk Names
main.js  950 bytes       0  [emitted]  main
Entrypoint main = main.js
[0] ./src/index.js 21 bytes {0} [built]
Johns-MBP:webpack-app admin$ npm i html-webpack-plugin html-loader --save-dev
npm WARN webpack-app@1.0.0 No description
npm WARN webpack-app@1.0.0 No repository field.

+ html-loader@0.5.5
+ html-webpack-plugin@3.2.0
added 45 packages from 60 contributors and audited 5765 packages in 4.725s
found 0 vulnerabilities

Johns-MBP:webpack-app admin$ npm run build

> webpack-app@1.0.0 build /Users/admin/GitHub/webpack-app
> webpack --mode production

Hash: 2ad06f44a285dfaae3fa
Version: webpack 4.25.0
Time: 504ms
Built at: 11/05/2018 7:23:37 AM
       Asset       Size  Chunks             Chunk Names
./index.html  519 bytes          [emitted]  
     main.js  950 bytes       0  [emitted]  main
Entrypoint main = main.js
[0] ./src/index.js 21 bytes {0} [built]
Child html-webpack-plugin for "index.html":
     1 asset
    Entrypoint undefined = ./index.html
    [0] ./node_modules/html-webpack-plugin/lib/loader.js!./src/index.html 516 bytes {0} [built]
Johns-MBP:webpack-app admin$ npm i webpack-dev-server --save-dev
npm WARN webpack-app@1.0.0 No description
npm WARN webpack-app@1.0.0 No repository field.

+ webpack-dev-server@3.1.10
added 127 packages from 102 contributors and audited 9202 packages in 6.79s
found 0 vulnerabilities

Johns-MBP:webpack-app admin$ npm i mini-css-extract-plugin css-loader --save-dev
npm WARN webpack-app@1.0.0 No description
npm WARN webpack-app@1.0.0 No repository field.

+ mini-css-extract-plugin@0.4.4
+ css-loader@1.0.1
added 27 packages from 49 contributors and audited 9334 packages in 5.14s
found 0 vulnerabilities

Johns-MBP:webpack-app admin$ npm run build

> webpack-app@1.0.0 build /Users/admin/GitHub/webpack-app
> webpack --mode production

Hash: c0a3e98b32c55ba35856
Version: webpack 4.25.0
Time: 781ms
Built at: 11/05/2018 7:29:45 AM
       Asset       Size  Chunks             Chunk Names
./index.html  558 bytes          [emitted]  
    main.css   30 bytes       0  [emitted]  main
     main.js  995 bytes       0  [emitted]  main
Entrypoint main = main.css main.js
[0] ./src/index.js 53 bytes {0} [built]
[1] ./src/main.css 39 bytes {0} [built]
    + 1 hidden module
Child html-webpack-plugin for "index.html":
     1 asset
    Entrypoint undefined = ./index.html
    [0] ./node_modules/html-webpack-plugin/lib/loader.js!./src/index.html 516 bytes {0} [built]
Child mini-css-extract-plugin node_modules/css-loader/index.js!src/main.css:
    Entrypoint mini-css-extract-plugin = *
    [0] ./node_modules/css-loader!./src/main.css 191 bytes {0} [built]
        + 1 hidden module
Johns-MBP:webpack-app admin$ npm run start

> webpack-app@1.0.0 start /Users/admin/GitHub/webpack-app
> webpack-dev-server --open --mode development

ℹ ｢wds｣: Project is running at http://localhost:8080/
ℹ ｢wds｣: webpack output is served from /
ℹ ｢wdm｣: Hash: 4bda6c7dc66a7ac3bad2
Version: webpack 4.25.0
Time: 1168ms
Built at: 11/05/2018 7:30:05 AM
       Asset       Size  Chunks             Chunk Names
./index.html  558 bytes          [emitted]  
    main.css   30 bytes    main  [emitted]  main
     main.js    343 KiB    main  [emitted]  main
Entrypoint main = main.css main.js
[0] multi (webpack)-dev-server/client?http://localhost:8080 ./src 40 bytes {main} [built]
[./node_modules/ansi-html/index.js] 4.16 KiB {main} [built]
[./node_modules/events/events.js] 8.13 KiB {main} [built]
[./node_modules/html-entities/index.js] 231 bytes {main} [built]
[./node_modules/loglevel/lib/loglevel.js] 7.68 KiB {main} [built]
[./node_modules/node-libs-browser/node_modules/punycode/punycode.js] 14.3 KiB {main} [built]
[./node_modules/url/url.js] 22.8 KiB {main} [built]
[./node_modules/webpack-dev-server/client/index.js?http://localhost:8080] (webpack)-dev-server/client?http://localhost:8080 7.78 KiB {main} [built]
[./node_modules/webpack-dev-server/client/overlay.js] (webpack)-dev-server/client/overlay.js 3.58 KiB {main} [built]
[./node_modules/webpack-dev-server/client/socket.js] (webpack)-dev-server/client/socket.js 1.05 KiB {main} [built]
[./node_modules/webpack-dev-server/node_modules/strip-ansi/index.js] (webpack)-dev-server/node_modules/strip-ansi/index.js 161 bytes {main} [built]
[./node_modules/webpack/hot sync ^\.\/log$] (webpack)/hot sync nonrecursive ^\.\/log$ 170 bytes {main} [built]
[./node_modules/webpack/hot/emitter.js] (webpack)/hot/emitter.js 75 bytes {main} [built]
[./src/index.js] 53 bytes {main} [built]
[./src/main.css] 39 bytes {main} [built]
    + 13 hidden modules
Child html-webpack-plugin for "index.html":
     1 asset
    Entrypoint undefined = ./index.html
    [./node_modules/html-webpack-plugin/lib/loader.js!./src/index.html] 516 bytes {0} [built]
Child mini-css-extract-plugin node_modules/css-loader/index.js!src/main.css:
    Entrypoint mini-css-extract-plugin = *
    [./node_modules/css-loader/index.js!./src/main.css] ./node_modules/css-loader!./src/main.css 191 bytes {mini-css-extract-plugin} [built]
    [./node_modules/css-loader/lib/css-base.js] 2.21 KiB {mini-css-extract-plugin} [built]
ℹ ｢wdm｣: Compiled successfully.

</pre>

![Alt text](./assets/image02.jpg?raw=true "AWS")
![Alt text](./assets/image01.jpg?raw=true "AWS")
![Alt text](./assets/image03.jpg?raw=true "AWS")
![Alt text](./assets/image04.jpg?raw=true "AWS")
