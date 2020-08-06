# TypeScript project starter pack

This is a small starter pack for getting a TypeScript project started using Webpack and ts-loader.
It also contains launch.json and tasks.json files for Visual Studio Code integration.

It is not meant to be super idiomatic or production ready. The goal is to have a base that is simple enough that you can build on top of it with confidence that you wont break something and not understand why.

## Usage

1. Clone this repository.
2. Run `npm install` in the cloned directory.
3. If using TSX but not using React, change the `jsxFactory` property in tsconfig.json.

If using VS Code and Google Chrome:

4. Press `ctrl-shift-p` and type in `Run task`. Press enter. Choose the `npm: start` task.
5. Press F5 to start debugging in Chrome.

Otherwise:

4. Open a terminal and execute `npm run start`
5. Open your web browser and go to http://localhost:8080/

Finally:

6. Start developing. The entry point for the application is src/index.ts.

## Running tests

Use the `start-test` npm task to start a Karma server that will watch files in src/ and test/ and run tests in modified files.

For testing, [Jasmine](https://jasmine.github.io/) + [Karma](https://karma-runner.github.io/2.0/index.html) is used.

## Prettier

[Prettier](https://prettier.io) is installed by default along with [lint-staged](https://github.com/okonet/lint-staged). This ensures that code in the repository has a coherent coding style. When committing to the repository, prettier will be ran against the staged files and will update them if there is any code in the files that violates the coding style.

For Visual Studio Code users, it is recommended to install the [prettier-vscode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) plugin. This will make the built in format on save functionality use prettier's coding style.

There are some alternatives listed [here](https://prettier.io/docs/en/editors.html) to run prettier on save in other editors.

Prettier is also ran in the `ci` GitHub Action which is included in this repository. The action will fail if you commit code that violates the coding style.
