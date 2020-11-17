# eslint issue 1086

A repository intended to replicate an issue with formatting files in the [dbaeumer.vscode-eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) vs code extension.

I am assuming this to be related to [issue #1086](https://github.com/microsoft/vscode-eslint/issues/1086), as it's the same error message, but this may be mistaken/the wrong call.

This repo contains `working.js`, which eslint formats as expected, and `broken.js` in the `/.example/` folder, which it does not.

### Version info

- Visual Studio Code v1.51.1 (64bit System Install on Windows 10)
- dbaeumer.vscode-eslint v2.1.13
- ESLint v7.13.0

### Screenshots

With eslint v7.11.0 or v7.13.0 installed globally:

![image](https://user-images.githubusercontent.com/52764066/99107569-ad2d6200-25ab-11eb-99df-54bbe65ee3e2.png)

With eslint v7.13.0 installed locally:

![image](https://user-images.githubusercontent.com/52764066/99337363-be929a80-2847-11eb-8eb7-d392f176a496.png)
