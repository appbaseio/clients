# Getting started

Appbase.io REST API

## How to Build


The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```PodFile``` file that comes with the SDK. 
To resolve these dependencies, we use the Cocoapods package manager.
Visit https://guides.cocoapods.org/using/getting-started.html to setup Cocoapods on your system.
Open command prompt and type ```pod --version```. This should display the current version of Cocoapods installed if the installation was successful.

Using command line, navigate to the directory containing the generated files (including ```PodFile```) for the SDK. 
Run the command ```pod install```. This should install all the required dependencies and create the ```pods``` directory in your project directory.

![Installing dependencies using Cocoapods](https://apidocs.io/illustration/objc?step=AddDependencies&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

Open the project workspace using the (AppbaseAPI.xcworkspace) file. Invoke the build process using `Command(⌘)+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Xcode](https://apidocs.io/illustration/objc?step=BuildSDK&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)


## How to Use

The generated code is a Cocoa Touch Static Library which can be used in any iOS project. The support for these generated libraries go all the way back to iOS 6.

The following section explains how to use the AppbaseAPI library in a new iOS project.     
### 1. Starting a new project
To start a new project, left-click on the ```Create a new Xcode project```.
![Create Test Project - Step 1](https://apidocs.io/illustration/objc?step=Test1&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

Next, choose **Single View Application** and click ```Next```.
![Create Test Project - Step 2](https://apidocs.io/illustration/objc?step=Test2&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

Provide **Test-Project** as the product name click ```Next```.
![Create Test Project - Step 3](https://apidocs.io/illustration/objc?step=Test3&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

Choose the desired location of your project folder and click ```Create```.
![Create Test Project - Step 4](https://apidocs.io/illustration/objc?step=Test4&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

### 2. Adding the static library dependency
To add this dependency open a terminal and navigate to your project folder. Next, input ```pod init``` and press enter.
![Add dependency - Step 1](https://apidocs.io/illustration/objc?step=Add0&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

Next, open the newly created ```PodFile``` in your favourite text editor. Add the following line : pod 'AppbaseAPI', :path => 'Vendor/AppbaseAPI'
![Add dependency - Step 2](https://apidocs.io/illustration/objc?step=Add1&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)

Execute `pod install` from terminal to install the dependecy in your project. This would add the dependency to the newly created test project.
![Add dependency - Step 3](https://apidocs.io/illustration/objc?step=Add2&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)


## How to Test

Unit tests in this SDK can be run using Xcode. 

First build the SDK as shown in the steps above and naivgate to the project directory and open the AppbaseAPI.xcworkspace file.

Go to the test explorer in Xcode as shown in the picture below and click on `run tests` from the menu. 
![Run tests](https://apidocs.io/illustration/objc?step=RunTests&workspaceFolder=Appbase%20API-ObjC&workspaceName=AppbaseAPI&projectName=AppbaseAPI&rootNamespace=AppbaseAPI)


## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| basicAuthUserName | The username to use with basic authentication |
| basicAuthPassword | The password to use with basic authentication |



Configuration variables can be set as following.
```Objc
// Configuration parameters and credentials
Configuration_BasicAuthUserName = "Configuration_BasicAuthUserName"; // The username to use with basic authentication
Configuration_BasicAuthPassword = "Configuration_BasicAuthPassword"; // The password to use with basic authentication

```

# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [IndexAPIsController](#index_ap_is_controller)

## <a name="index_ap_is_controller"></a>![Class: ](https://apidocs.io/img/class.png ".IndexAPIsController") IndexAPIsController

### Get singleton instance
```objc
IndexAPIs* indexAPIs = [[IndexAPIs alloc]init] ;
```

### <a name="g_et_app_async_with_app"></a>![Method: ](https://apidocs.io/img/method.png ".IndexAPIsController.gETAppAsyncWithApp") gETAppAsyncWithApp

> Informational endpoint.


```objc
function gETAppAsyncWithApp:(NSString*) app
                completionBlock:(CompletedGETApp) onCompleted(app)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* app = @"app";

    [self.indexAPIs gETAppAsyncWithApp: app  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)



