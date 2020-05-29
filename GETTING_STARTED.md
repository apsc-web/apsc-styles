## 🔎 Getting Started

- [VSCode](#vscode)
- [Install Dependencies](#install-dependencies)
- [Create Your First Project](#create-your-first-project)
- [Command Line Tool](#command-line-tools)
- [Start Local Server](#start-local-server)

## VSCode

APSC recommends using [VSCode](https://code.visualstudio.com/) as your code editor.

The following extensions are recommended:

* [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) - Launch a local development server with live reload feature for static & dynamic pages.
* [Beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify) - Beautify your ugly code.
* [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) - Quickly glimpse into whom, why, and when a line or code block was changed.

<br />

## Install Dependencies

Run the following in the repository root

```bash
npm install
```

Sass will be installed as a dependency to compile SCSS to CSS.

<br />

## Create Your First Project

To create a new project:

```bash
npm run create-project --project=<project-name>
```

A new project will be created in apsc-scss with your project name

<br />

## Command Line Tools

To watch your project SCSS:

```bash
npm run watch --project=<project-name>
```
Sass will watch for any changes to SCSS files in the project folder, it will get compiled into the dev.css in the dev folder.  

<br />

To compile and minify your project CSS

```bash
npm run compile --project=<project-name>
```

A minified project CSS file will be created in the dist folder.

<br />

## Start Local Server

Open ```index.html``` page in the dev folder and the start the local server using the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Extension (bottom bar in VSCode editor window). The local server will automatically watch for any changes in your SCSS code.