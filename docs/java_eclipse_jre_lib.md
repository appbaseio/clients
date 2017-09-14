# Getting started

Appbase.io REST API

## How to Build

The generated code uses a few Maven dependencies e.g., Jackson, UniRest,
and Apache HttpClient. The reference to these dependencies is already
added in the pom.xml file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Eclipse click on ``` File -> Import ```.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/java?step=import0&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

* In the import dialog, select ``` Existing Java Project ``` and click ``` Next ```.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/java?step=import1&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

* Browse to locate the folder containing the source code. Select the detected location of the project and click ``` Finish ```.

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/java?step=import2&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

* Upon successful import, the project will be automatically built by Eclipse after automatically resolving the dependencies.

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/java?step=import3&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

## How to Use

The following section explains how to use the AppbaseAPI library in a new console project.

### 1. Starting a new project

For starting a new project, click the menu command ``` File > New > Project ```.

![Add a new project in Eclipse](https://apidocs.io/illustration/java?step=createNewProject0&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Next, choose ``` Maven > Maven Project ```and click ``` Next ```.

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/java?step=createNewProject1&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Here, make sure to use the current workspace by choosing ``` Use default Workspace location ```, as shown in the picture below and click ``` Next ```.

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/java?step=createNewProject2&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Following this, select the *quick start* project type to create a simple project with an existing class and a ``` main ``` method. To do this, choose ``` maven-archetype-quickstart ``` item from the list and click ``` Next ```.

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/java?step=createNewProject3&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

In the last step, provide a ``` Group Id ``` and ``` Artifact Id ``` as shown in the picture below and click ``` Finish ```.

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/java?step=createNewProject4&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

### 2. Add reference of the library project

The created Maven project manages its dependencies using its ``` pom.xml ``` file. In order to add a dependency on the *AppbaseAPILib* client library, double click on the ``` pom.xml ``` file in the ``` Package Explorer ```. Opening the ``` pom.xml ``` file will render a graphical view on the cavas. Here, switch to the ``` Dependencies ``` tab and click the ``` Add ``` button as shown in the picture below.

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/java?step=testProject0&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

Clicking the ``` Add ``` button will open a dialog where you need to specify AppbaseAPI in ``` Group Id ``` and AppbaseAPILib in the ``` Artifact Id ``` fields. Once added click ``` OK ```. Save the ``` pom.xml ``` file.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject1&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

### 3. Write sample code

Once the ``` SimpleConsoleApp ``` is created, a file named ``` App.java ``` will be visible in the *Package Explorer* with a ``` main ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject2&workspaceFolder=Appbase%20API-Java&workspaceName=AppbaseAPI&projectName=AppbaseAPILib&rootNamespace=io.appbase.api.scalr)

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project *AppbaseAPILib* from the package explorer.
2. Select "Run -> Run as -> JUnit Test" or use "Alt + Shift + X" followed by "T" to run the Tests.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| username | username is the first part of the credentials (before ':') |
| password | password is the second part of the credentials (after ':') |



API client can be initialized as following.

```java
// Configuration parameters and credentials
String username = "TODO: Replace this"; // username is the first part of the credentials (before ':')
String password = "TODO: Replace this"; // password is the second part of the credentials (after ':')

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



