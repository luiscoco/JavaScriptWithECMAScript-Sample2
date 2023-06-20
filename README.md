# JavaScript with ECMAScript. Sample2 with no html pages.

## 1.Create a package.json file:
In your project folder, open the terminal in VSCode and run the following command to initialize a package.json file:
```
npm init -y
```
This will create a basic package.json file in your project folder.

## 2.Modify the package.json file: 
Open the package.json file and add the following line within the JSON object:

```json
{
  "name": "sample2-javascript",
  "version": "1.0.0",
  "type": "module",
  "description": "",
  "main": "app.js",
  "scripts": {
    "start": "node app.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC" 
}
```

We added the line: "type": "module", and the line: "start": "node app.js"

## 3.To run the application:
```
node app.js
```

## 4.(Optional)
Modify the file extensions: Rename the app.js file to app.mjs, and rename the greeting.js file to greeting.mjs.
Update the import statement in app.mjs: Change the import statement in app.mjs to use the .mjs extension for the module file:
```javascript
import { greet } from './greeting.mjs';
```

Update the script in package.json: In the "scripts" section of package.json, update the "start" script to point to the app.mjs file:
```
"scripts": {
  "start": "node --experimental-modules app.mjs"
}
```

Run the application: Open the terminal in VSCode and run the following command:
```
npm start
```

This command will execute the start script defined in package.json, running the application with the app.mjs file as the entry point.


