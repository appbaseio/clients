# Getting started

Appbase.io REST API

## How to Build

The generated SDK relies on [Node Package Manager](https://www.npmjs.com/) (NPM) being available to resolve dependencies. If you don't already have NPM installed, please go ahead and follow instructions to install NPM from [here](https://nodejs.org/en/download/).
The SDK also requires Node to be installed. If Node isn't already installed, please install it from [here](https://nodejs.org/en/download/)
> NPM is installed by default when Node is installed

To check if node and npm have been successfully installed, write the following commands in command prompt:

* `node --version`
* `npm -version`

![Version Check](https://apidocs.io/illustration/nodejs?step=versionCheck&workspaceFolder=Appbase%20API-Node)

Now use npm to resolve all dependencies by running the following command in the root directory (of the SDK folder):

```bash
npm install
```

![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency1&workspaceFolder=Appbase%20API-Node)

![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency2)

This will install all dependencies in the `node_modules` folder.

Once dependencies are resolved, you will need to move the folder `AppbaseAPILib ` in to your `node_modules` folder.

## How to Use

The following section explains how to use the library in a new project.

### 1. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

Click on `File` and select `Open Folder`.

![Open Folder](https://apidocs.io/illustration/nodejs?step=openFolder)

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.

![Open Project](https://apidocs.io/illustration/nodejs?step=openProject&workspaceFolder=Appbase%20API-Node)

### 2. Creating a Test File

Now right click on the folder name and select the `New File` option to create a new test file. Save it as `index.js` Now import the generated NodeJS library using the following lines of code:

```js
var lib = require('lib');
```

Save changes.

![Create new file](https://apidocs.io/illustration/nodejs?step=createNewFile&workspaceFolder=Appbase%20API-Node)

![Save new file](https://apidocs.io/illustration/nodejs?step=saveNewFile&workspaceFolder=Appbase%20API-Node)

### 3. Running The Test File

To run the `index.js` file, open up the command prompt and navigate to the Path where the SDK folder resides. Type the following command to run the file:

```
node index.js
```

![Run file](https://apidocs.io/illustration/nodejs?step=runProject&workspaceFolder=Appbase%20API-Node)


## How to Test

These tests use Mocha framework for testing, coupled with Chai for assertions. These dependencies need to be installed for tests to run.
Tests can be run in a number of ways:

### Method 1 (Run all tests)

1. Navigate to the root directory of the SDK folder from command prompt.
2. Type `mocha --recursive` to run all the tests.

### Method 2 (Run all tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha *` to run all the tests.

### Method 3 (Run specific controller's tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha  Appbase APIController`  to run all the tests in that controller file.

> To increase mocha's default timeout, you can change the `TEST_TIMEOUT` parameter's value in `TestBootstrap.js`.

![Run Tests](https://apidocs.io/illustration/nodejs?step=runTests&controllerName=Appbase%20APIController)

## Initialization

### Authentication
In order to setup authentication in the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| username | username is the first part of the credentials (before ':') |
| password | password is the second part of the credentials (after ':') |



API client can be initialized as following:

```JavaScript
const lib = require('lib');

// Configuration parameters and credentials
lib.Configuration.username = "TODO: Replace this"; // username is the first part of the credentials (before ':')
lib.Configuration.password = "TODO: Replace this"; // password is the second part of the credentials (after ':')

```



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AppController](#app_controller)

## <a name="app_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AppController") AppController

### Get singleton instance

The singleton instance of the ``` AppController ``` class can be accessed from the API Client.

```javascript
var controller = lib.AppController;
```

### <a name="g_et_app"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.gETApp") gETApp

> Informational endpoint.


```javascript
function gETApp(app, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |



#### Example Usage

```javascript

    var app = 'app';

    controller.gETApp(app, function(error, response, context) {

    
    });
```



### <a name="g_et_app_settings"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.gETAppSettings") gETAppSettings

> Get settings in an app


```javascript
function gETAppSettings(app, queryParams, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |



#### Example Usage

```javascript

    var app = 'app';

    // key-value map for optional query parameters
    var queryParams = [];

    controller.gETAppSettings(app, queryParams, function(error, response, context) {

    
    });
```



### <a name="g_et_app_mappings"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.gETAppMappings") gETAppMappings

> Get an app's mappings.


```javascript
function gETAppMappings(app, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |



#### Example Usage

```javascript

    var app = 'app';

    controller.gETAppMappings(app, function(error, response, context) {

    
    });
```



[Back to List of Controllers](#list_of_controllers)



