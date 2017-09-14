# Getting started

Appbase.io REST API

## How to Build

This client library is a Ruby gem which can be compiled and used in your Ruby and Ruby on Rails project. This library requires a few gems from the RubyGems repository.

1. Open the command line interface or the terminal and navigate to the folder containing the source code.
2. Run ``` gem build appbase_api.gemspec ``` to build the gem.
3. Once built, the gem can be installed on the current work environment using ``` gem install appbase_api-1.0.0.gem ```

![Building Gem](https://apidocs.io/illustration/ruby?step=buildSDK&workspaceFolder=Appbase%20API-Ruby&workspaceName=Appbase%20API-Ruby&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

## How to Use

The following section explains how to use the AppbaseApi Ruby Gem in a new Rails project using RubyMine&trade;. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

### 1. Starting a new project

Close any existing projects in RubyMine&trade; by selecting ``` File -> Close Project ```. Next, click on ``` Create New Project ``` to create a new project from scratch.

![Create a new project in RubyMine](https://apidocs.io/illustration/ruby?step=createNewProject0&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

Next, provide ``` TestApp ``` as the project name, choose ``` Rails Application ``` as the project type, and click ``` OK ```.

![Create a new Rails Application in RubyMine - step 1](https://apidocs.io/illustration/ruby?step=createNewProject1&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

In the next dialog make sure that correct *Ruby SDK* is being used (minimum 2.0.0) and click ``` OK ```.

![Create a new Rails Application in RubyMine - step 2](https://apidocs.io/illustration/ruby?step=createNewProject2&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

This will create a new Rails Application project with an existing set of files and folder.

### 2. Add reference of the gem

In order to use the AppbaseApi gem in the new project we must add a gem reference. Locate the ```Gemfile``` in the *Project Explorer* window under the ``` TestApp ``` project node. The file contains references to all gems being used in the project. Here, add the reference to the library gem by adding the following line: ``` gem 'appbase_api', '~> 1.0.0' ```

![Add references of the Gemfile](https://apidocs.io/illustration/ruby?step=addReference&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

### 3. Adding a new Rails Controller

Once the ``` TestApp ``` project is created, a folder named ``` controllers ``` will be visible in the *Project Explorer* under the following path: ``` TestApp > app > controllers ```. Right click on this folder and select ``` New -> Run Rails Generator... ```.

![Run Rails Generator on Controllers Folder](https://apidocs.io/illustration/ruby?step=addCode0&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

Selecting the said option will popup a small window where the generator names are displayed. Here, select the ``` controller ``` template.

![Create a new Controller](https://apidocs.io/illustration/ruby?step=addCode1&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

Next, a popup window will ask you for a Controller name and included Actions. For controller name provide ``` Hello ``` and include an action named ``` Index ``` and click ``` OK ```.

![Add a new Controller](https://apidocs.io/illustration/ruby?step=addCode2&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

A new controller class anmed ``` HelloController ``` will be created in a file named ``` hello_controller.rb ``` containing a method named ``` Index ```. In this method, add code for initialization and a sample for its usage.

![Initialize the library](https://apidocs.io/illustration/ruby?step=addCode3&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0)

## How to Test

You can test the generated SDK and the server with automatically generated test
cases as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke: `bundle exec rake`

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| username | username is the first part of the credentials (before ':') |
| password | password is the second part of the credentials (after ':') |



API client can be initialized as following.

```ruby
# Configuration parameters and credentials
username = 'TODO: Replace this' # username is the first part of the credentials (before ':')
password = 'TODO: Replace this' # password is the second part of the credentials (after ':')

client = AppbaseApi::AppbaseApiClient.new(
  username: username,
  password: password
)
```

The added initlization code can be debugged by putting a breakpoint in the ``` Index ``` method and running the project in debug mode by selecting ``` Run -> Debug 'Development: TestApp' ```.

![Debug the TestApp](https://apidocs.io/illustration/ruby?step=addCode4&workspaceFolder=Appbase%20API-Ruby&workspaceName=AppbaseApi&projectName=appbase_api&gemName=appbase_api&gemVer=1.0.0&initLine=client%2520%253D%2520AppbaseApiClient.new%2528%2527username%2527%252C%2520%2527password%2527%2529)



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AppController](#app_controller)

## <a name="app_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AppController") AppController

### Get singleton instance

The singleton instance of the ``` AppController ``` class can be accessed from the API Client.

```ruby
app = client.app
```

### <a name="get_app"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.get_app") get_app

> Informational endpoint.


```ruby
def get_app(app); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |


#### Example Usage

```ruby
app = 'app'

result = app.get_app(app)

```


### <a name="get_app__settings"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.get_app__settings") get_app__settings

> Get settings in an app


```ruby
def get_app__settings(app,
                          _query_parameters = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |
| _query_parameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```ruby
app = 'app'
# key-value map for optional query parameters
queryParams = { 'key' => 'value' }

result = app.get_app__settings(app, queryParams)

```


### <a name="get_app__mappings"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.get_app__mappings") get_app__mappings

> Get an app's mappings.


```ruby
def get_app__mappings(app); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |


#### Example Usage

```ruby
app = 'app'

result = app.get_app__mappings(app)

```


[Back to List of Controllers](#list_of_controllers)



