# Azure Data Studio Debug

This extension forms the [Azure Data Studio](https://docs.microsoft.com/en-us/sql/azure-data-studio) extension debugging experience.

# Release Notes

## 1.2
Renamed the extension to Azure Data Studio Debug, matching the rename of Azure Data Studio (previously known as SQL Operations Studio).

## 1.0.2
Fixed issue where use of the `sqlops` default runtimeExecutable target didn't work as expected. Testing of this has been verified on macOS and Windows, but not Linux.


# Building and debugging an extension

## Prerequisites
To develop an extension you need [Node.js](https://nodejs.org/en/) installed and available in your `$PATH`. Node.js includes [npm](https://www.npmjs.com/), the Node.js Package Manager, which will be used to install the extension generator.

## Install the extension generator
Install Yeoman and the Azure Data Studio Extension generator from the command prompt:

```sh
npm install -g yo generator-sqlops
```

## Run yo sqlops
The Yeoman generator will walk you through the steps required to create your customization or extension prompting for the required information.

To launch the generator, type the following in a command prompt:

```sh
yo sqlops
```

##  Generate a new extension
Pick the `New Extension (Typescript)` option to quickly get started with an extension

## Debug your extension
* Press `F5` or click the `Debug` icon and click `Start`
* A new instance of Azure Data Studio will start in a special mode (`Extension Development Host`) and *this new instance is now aware of your extension*.
* Press `ctrl+shift+P` (Windows/Linux) or `cmd+shift+P` (macOS) and run the command named Hello World.
* Congratulations! You've just created and executed your first Azure Data Studio command!

You can now add breakpoints to your code and debug as needed.

## Next steps
Take a look at the [extension samples](https://github.com/Microsoft/sqlopsstudio/tree/master/samples) for examples of the type of extension points added to Azure Data Studio. Also look at the [VSCode Extensibility Reference](https://code.visualstudio.com/docs/extensions/overview) - most of the extension points will work, with the exclusion of the debug namespace.

Contact the team on [gitter](https://gitter.im/Microsoft/sqlopsstudio) or via our [issues page](https://github.com/Microsoft/sqlopsstudio/issues) if you have questions on adding extensions.

See a general overview of debugging in VS Code [here](https://code.visualstudio.com/docs/editor/debugging).

# License

Copyright (c) Microsoft. All rights reserved.

Licensed under the [MIT](LICENSE.txt) License.
