# TypeScript NPM Package Template
Scaffold NPM Package using TypeScript and Parcel.

This project includes:
- [TypeScript](https://www.typescriptlang.org/)
- [Parcel](https://parceljs.org/)
- [TypeDoc](https://typedoc.org/)

## Getting Started

Begin via any of the following:

- Press the "*Use this template*" button

- Use [degit](https://github.com/fabiofranzini/typescript-npm-package-template) to execute: 

    ```
    degit github:fabiofranzini/typescript-npm-package-template
    ```
    
- Use [GitHub CLI](https://cli.github.com/) to execute: 

    ```
    gh repo create <name> --template="https://github.com/fabiofranzini/typescript-npm-package-template"
    ```
    
- Simply `git clone`, delete the existing .git folder, and then:

    ```
    git init
    git add -A
    git commit -m "Initial commit"
    ````

- Change the informations in the package.json file

Remember to use `npm search <term>` to avoid naming conflicts in the NPM Registery for your new package name.

## Usage

The following tasks are available for `npm run`:

- `watch`: Run Parcel in watch mode to detect changes to files during development
- `build`: Run Parcel to build a production release distributable with source maps
- `release`: Run Parcel to build a production release distributable without source maps
- `docs`: Run TypeDoc for TSDoc generated documentation in the "*docs/*" folder
- `clean`: Remove all files from the "*dist/*" and "*docs/*" folders

## Release Publishing

Update your `package.json` to next version number, and remember to tag a release.

Once ready to submit your package to the NPM Registry, execute the following tasks via `npm` (or `yarn`):

- `npm run release` &mdash; Assure a clean release build wihtout source maps

Assure the proper npm login:

```
npm login
```

Submit your package to the registry:

```
npm publish --access public
```