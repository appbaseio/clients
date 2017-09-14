# Getting started

Appbase.io REST API

## How to Build

The generated code uses a few Gradle dependencies e.g., Jackson, Volley,
and Apache HttpClient. The reference to these dependencies is already
added in the build.gradle file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Android Studio click on ``` Open an Existing Android Project ```.

![Importing SDK into Android Studio - Step 1](https://apidocs.io/illustration/android?step=import1&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

* Browse to locate the folder containing the source code. Select the location of the AppbaseAPI gradle project and click ``` Ok ```.

![Importing SDK into Android Studio - Step 2](https://apidocs.io/illustration/android?step=import2&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

* Upon successful import, the project can be built by clicking on ``` Build > Make Project ``` or  pressing ``` Ctrl + F9 ```.

![Importing SDK into Android Studio - Step 3](https://apidocs.io/illustration/android?step=import3&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

## How to Use

The following section explains how to use the AppbaseAPI library in a new project.

### 1. Starting a new project 

For starting a new project, click on ``` Create New Android Studio Project ```.

![Add a new project in Android Studio - Step 1](https://apidocs.io/illustration/android?step=createNewProject0&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Here, configure the new project by adding the name, domain and location of the sample application followed by clicking ``` Next ```.

![Create a new Android Studio Project - Step 2](https://apidocs.io/illustration/android?step=createNewProject1&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Following this, select the `Phone and Tablet` option as shown in the illustration below and click `Next`.

![Create a new Android Studio Project - Step 3](https://apidocs.io/illustration/android?step=createNewProject2&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

In the following step, choose ``` Empty Activity ``` as the activity type and click ``` Next ```.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject3&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

In this step, provide an ``` Activity Name ``` and ``` Layout Name ``` and click ``` Finish ```.  This would take you to the newly created project.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject4&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

### 2. Add reference of the library project

In order to add a dependency to this sample application, click on the android button shown in the project explorer on the left side as shown in the picture. Click on ``` Project ``` in the drop down that emerges.  

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/android?step=testProject0&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Right click the sample application in the project explorer and click on ``` New > Module ```  as shown in the picture.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/android?step=testProject1&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Choose ``` Import Gradle Project ``` and click ``` Next ```.

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/android?step=testProject2&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Click on ``` Finish ``` which would take you back to the sample application with the refernced SDK. 

![Adding dependency to the client library - Step 4](https://apidocs.io/illustration/android?step=testProject3&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

In the following step naigate to the ``` SampleApplication >  app > build.gradle ``` file and add the following line ```compile project(path: ':AppbaseAPI')``` to the dependencies section as shown in the illustration below.

![Adding dependency to the client library - Step 5](https://apidocs.io/illustration/android?step=testProject4&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Finally, press ``` Sync Now ``` in the warning visible as shown in the picture below.

![Adding dependency to the client library - Step 6](https://apidocs.io/illustration/android?step=testProject5&workspaceFolder=Appbase%20API&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

### 3. Write sample code

Once the ``` SampleApplication ``` is created, a file named ``` SampleApplication > app > src > main > java > MainActivity ``` will be visible in the *Project Explorer* with an ``` onCreate ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Android Studio, for running the tests do the following:

1. Right click on *SampleApplication > AppbaseAPILib > androidTest > java)* from the project explorer.
2. Select "Run All Tests" or use "Ctrl + Shift + F10" to run the Tests.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| username | username is the first part of the credentials (before ':') |
| password | password is the second part of the credentials (after ':') |



API client can be initialized as following. The `appContext` being passed is the Android application [`Context`](https://developer.android.com/reference/android/content/Context.html).

```java
// Configuration parameters and credentials
String username = "TODO: Replace this"; // username is the first part of the credentials (before ':')
String password = "TODO: Replace this"; // password is the second part of the credentials (after ':')

io.appbase.api.scalr.Configuration.initialize(appContext);
AppbaseAPIClient client = new AppbaseAPIClient(username, password);
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AppController](#app_controller)

## <a name="app_controller"></a>![Class: ](https://apidocs.io/img/class.png "io.appbase.api.scalr.controllers.AppController") AppController

### Get singleton instance

The singleton instance of the ``` AppController ``` class can be accessed from the API Client.

```java
AppController app = client.getApp();
```

### <a name="g_et_app_async"></a>![Method: ](https://apidocs.io/img/method.png "io.appbase.api.scalr.controllers.AppController.gETAppAsync") gETAppAsync

> Informational endpoint.


```java
void gETAppAsync(
        final String app,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |


#### Example Usage

```java
String app = "app";
// Invoking the API call with sample inputs
app.gETAppAsync(app, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="g_et_app_settings_async"></a>![Method: ](https://apidocs.io/img/method.png "io.appbase.api.scalr.controllers.AppController.gETAppSettingsAsync") gETAppSettingsAsync

> Get settings in an app


```java
void gETAppSettingsAsync(
        final String app,
        Map<String, Object> queryParameters,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```java
String app = "app";
// key-value map for optional query parameters
Map<String, Object> queryParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
app.gETAppSettingsAsync(app, queryParams, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="g_et_app_mappings_async"></a>![Method: ](https://apidocs.io/img/method.png "io.appbase.api.scalr.controllers.AppController.gETAppMappingsAsync") gETAppMappingsAsync

> Get an app's mappings.


```java
void gETAppMappingsAsync(
        final String app,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |


#### Example Usage

```java
String app = "app";
// Invoking the API call with sample inputs
app.gETAppMappingsAsync(app, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)



