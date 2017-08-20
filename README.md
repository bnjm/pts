# Pts

![image](./guide/assets/pts.png)
Pts is a new typescript/es6 library that enables you to compose and visualize points in spaces.

This project is currently still in development. Almost there!

Take a peek at [ptsjs.org](https://ptsjs.org)


## Usage
**Option 1:** Download the [latest release](https://github.com/williamngan/pts/releases) and use `dist/pts.min.js` directly. 
```
<script type="text/javascript" src="pts.min.js"></script>
```
Pts is pretty lightweight. Currently at ~16kb when minified and gzipped.

**Option 2:** Install via `npm install pts`. Then you can choose to import some parts of Pts into your project as needed. 
```
import {CanvasSpace, Pt, Group, Line} from 'pts';
```
See this example of using Pts in a React component [here](https://github.com/williamngan/pts-react-example).


## For development
Pts is written in typescript. You can clone or fork this project and build it as follows:

### Build and test

Clone this repo and install dependencies via `npm install`.

```
npm start
npm run build
npm test
```

### Generate documentations
```
typedoc --readme none --out docs src --name Pts
```

### Generate typescript declaration files
```
tsc
dts-bundle --name pts --main dist/files/*.d.ts --out ../pts.d.ts
```

## License
Apache License 2.0. See LICENSE file for details.   
Copyright © 2017 by William Ngan and contributors.