# ArcGIS API for JavaScript Template Application

## Usage

### Step 1: Install Homebrew
Homebrew is a package manager for Mac and helps to easily install and uninstall softwares on a Mac.

#### To install Homebrew run the following command in the terminal.

_$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"_
For more detail on Homebrew check their website.

Once you have homebrew installed on your system you can use it to install many packages.

### Step 2: Install Node
By installing NodeJS you will also get NPM which is Node package manager. It will help you to install other packages.

#### To install Node on your Mac using Homebrew type the following command.

_$ brew install node_
Once you have Node installed you can check its version by typing the following command in the terminal.

_$ node -v_
And, to check the version of NPM type the following command in the terminal.

-$ npm -v_
Click here to read the tutorial on How to install NodeJS on Mac.

So, now we have Node and NPM installed on our system. Time to install TypeScript using NPM.

### Step 3: Install TypeScript
We will install TypeScript globally on our Mac so that we can access it from any directory. For this we will use the following command.

_$ sudo npm install -g typescript_
You may have to use sudo if you don't have permissions.

#### Output

YUSUF-MacBook-Pro:~ yusufshakeel$ sudo npm install -g typescript
Password:
/usr/local/bin/tsc -> /usr/local/lib/node_modules/typescript/bin/tsc
/usr/local/bin/tsserver -> /usr/local/lib/node_modules/typescript/bin/tsserver
/usr/local/lib
└── typescript@2.2.1 

YUSUF-MacBook-Pro:~ yusufshakeel$

#### Once you have TypeScript installed use the following command to check the version.

_$ tsc -v_

#### Output

YUSUF-MacBook-Pro:~ yusufshakeel$ tsc -v
Version 2.2.1
YUSUF-MacBook-Pro:~ yusufshakeel$
Using TypeScript to convert .TS file into .JS file
Lets say, we have a project folder example and we have an app.ts TypeScript file which we want to convert into JavaScript file.

The content of app.ts file is given below.

console.log("Hello World!");

### To convert app.ts file into app.js file we use the following command in the terminal.

_$ tsc app.ts_

#### Output

YUSUF-MacBook-Pro:~ yusufshakeel$ cd Documents/yusuf-dev/
YUSUF-MacBook-Pro:yusuf-dev yusufshakeel$ mkdir example
YUSUF-MacBook-Pro:yusuf-dev yusufshakeel$ cd example/
YUSUF-MacBook-Pro:example yusufshakeel$ vi app.ts
YUSUF-MacBook-Pro:example yusufshakeel$ tsc app.ts
YUSUF-MacBook-Pro:example yusufshakeel$ ls -la
total 16
drwxr-xr-x  4 yusufshakeel  staff  136 Mar 13 09:06 .
drwxr-xr-x  8 yusufshakeel  staff  272 Mar 13 09:05 ..
-rw-r--r--  1 yusufshakeel  staff   28 Mar 13 09:06 app.js
-rw-r--r--  1 yusufshakeel  staff   28 Mar 13 09:06 app.ts
YUSUF-MacBook-Pro:example yusufshakeel$

## Uninstall TypeScript

### To uninstall TypeScript globally we use the following command.

_$ sudo npm uninstall -g typescript_

You may have to use sudo if you don't have the permissions.

### Output

YUSUF-MacBook-Pro:~ yusufshakeel$ sudo npm uninstall -g typescript
Password:
- typescript@2.2.1 node_modules/typescript
YUSUF-MacBook-Pro:~ yusufshakeel$
And that's all for this tutorial. Have fun coding.


This application is written in [TypeScript](http://www.typescriptlang.org/) and utilizes the [`@arcgis/webpack-plugin`](https://github.com/Esri/arcgis-webpack-plugin).

You can develop, test, and build the application using various commands.

Run the application in development mode with a local development server.
```sh
npm start
```

Run the unit tests for the application. Unit tests are written with [Jest](https://jestjs.io/).
```sh
npm test
```

Build the application for deployment.
```sh
npm run build
```

Run a production build of the application, but serve it up locally to see how the built app will behave.
```sh
npm run serve
```

Use `npm run serve` to full test that Service Workers are working correctly with `webpack-dev-server` self signed certifcates. Refer to [this article](https://deanhume.com/testing-service-workers-locally-with-self-signed-certificates/) on how to run Chrome with proper flags enabled for development purposes.
