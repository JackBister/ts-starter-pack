# TypeScript project starter pack
This is a small starter pack for getting a TypeScript project started using Webpack and ts-loader.
It also contains launch.json and tasks.json files for Visual Studio Code integration.

It is not meant to be super idiomatic or production ready. The goal is to have a base that is simple enough that you can build on top of it with confidence that you wont break something and not understand why.

## Usage
1. Clone this repository.
2. Run ```npm install``` in the cloned directory.
3. If using TSX but not using React, change the ```jsxFactory``` property in tsconfig.json.

If using VS Code and Google Chrome:

4. Press ```ctrl-shift-p``` and type in ```Run task```. Press enter. Choose the ```npm: start``` task.
5. Press F5 to start debugging in Chrome.

Otherwise:

4. Open a terminal and execute ```npm run start```
5. Open your web browser and go to http://localhost:8080/

Finally:

6. Start developing. The entry point for the application is src/index.ts.
