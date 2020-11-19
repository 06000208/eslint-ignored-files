# eslint ignored files

A repository which replicates files and folders starting with a period being ignored, resulting in a cannot format error when using the vsc eslint extension 

It contains `working.js`, which formats as expected, and `ignored.js` in the `/.example/` folder, which does not.

See:

- https://github.com/microsoft/vscode-eslint/issues/550
- https://github.com/microsoft/vscode-eslint/issues/1086#issuecomment-728775230
- https://github.com/eslint/eslint/issues/8429

This can be resolved via:

> If anyone else gets here via Google trying to figure out why dot folders are ignored, you can fix it by adding a negating ignore in your `.eslintignore`:
> 
> ```
> !/.storybook
> ```
> 
> Now anything like `.storybook/config.js` will be included in the lint.

[_Originally posted by @bbugh_](https://github.com/eslint/eslint/issues/8429#issuecomment-355967308)

### Version info

- Visual Studio Code v1.51.1 (64bit System Install on Windows 10)
- dbaeumer.vscode-eslint v2.1.13
- ESLint v7.13.0

### Screenshots

![eslint v7.11.0 or v7.13.0 installed globally](https://user-images.githubusercontent.com/52764066/99107569-ad2d6200-25ab-11eb-99df-54bbe65ee3e2.png)

![eslint v7.13.0 installed locally](https://user-images.githubusercontent.com/52764066/99337363-be929a80-2847-11eb-8eb7-d392f176a496.png)
