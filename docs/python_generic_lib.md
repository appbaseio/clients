# Getting started

Appbase.io REST API

## How to Build


You must have Python 2 >=2.7.9 or Python 3 >=3.4 installed on your system to install and run this SDK. This SDK package depends on other Python packages like nose, jsonpickle etc. 
These dependencies are defined in the ```requirements.txt``` file that comes with the SDK.
To resolve these dependencies, you can use the PIP Dependency manager. Install it by following steps at [https://pip.pypa.io/en/stable/installing/](https://pip.pypa.io/en/stable/installing/).

Python and PIP executables should be defined in your PATH. Open command prompt and type ```pip --version```.
This should display the version of the PIP Dependency Manager installed if your installation was successful and the paths are properly defined.

* Using command line, navigate to the directory containing the generated files (including ```requirements.txt```) for the SDK.
* Run the command ```pip install -r requirements.txt```. This should install all the required dependencies.

![Building SDK - Step 1](https://apidocs.io/illustration/python?step=installDependencies&workspaceFolder=Appbase%20API-Python)


## How to Use

The following section explains how to use the Appbaseapi SDK package in a new project.

### 1. Open Project in an IDE

Open up a Python IDE like PyCharm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=pyCharm)

Click on ```Open``` in PyCharm to browse to your generated SDK directory and then click ```OK```.

![Open project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=openProject0&workspaceFolder=Appbase%20API-Python)     

The project files will be displayed in the side bar as follows:

![Open project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=openProject1&workspaceFolder=Appbase%20API-Python&projectName=appbaseapi)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=createDirectory&workspaceFolder=Appbase%20API-Python&projectName=appbaseapi)

Name the directory as "test"

![Add a new project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=nameDirectory)
   
Add a python file to this project with the name "testsdk"

![Add a new project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=createFile&workspaceFolder=Appbase%20API-Python&projectName=appbaseapi)

Name it "testsdk"

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=nameFile)

In your python file you will be required to import the generated python library using the following code lines

```Python
from appbaseapi.appbaseapi_client import AppbaseapiClient
```

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=projectFiles&workspaceFolder=Appbase%20API-Python&libraryName=appbaseapi.appbaseapi_client&projectName=appbaseapi)

After this you can write code to instantiate an API client object, get a controller object and  make API calls. Sample code is given in the subsequent sections.

### 3. Run the Test Project

To run the file within your test project, right click on your Python file inside your Test project and click on ```Run```

![Run Test Project - Step 1](https://apidocs.io/illustration/python?step=runProject&workspaceFolder=Appbase%20API-Python&libraryName=appbaseapi.appbaseapi_client&projectName=appbaseapi)


## How to Test

You can test the generated SDK and the server with automatically generated test
cases. unittest is used as the testing framework and nose is used as the test
runner. You can run the tests as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke 'pip install -r test-requirements.txt'
  3. Invoke 'nosetests'

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| username | username is the first part of the credentials (before ':') |
| password | password is the second part of the credentials (after ':') |



API client can be initialized as following.

```python
# Configuration parameters and credentials
username = 'TODO: Replace this' # username is the first part of the credentials (before ':')
password = 'TODO: Replace this' # password is the second part of the credentials (after ':')

client = AppbaseapiClient(username, password)
```



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AppController](#app_controller)

## <a name="app_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AppController") AppController

### Get controller instance

An instance of the ``` AppController ``` class can be accessed from the API Client.

```python
 app_client = client.app
```

### <a name="get_app"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.get_app") get_app

> Informational endpoint.

```python
def get_app(self,
                app)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |



#### Example Usage

```python
app = 'app'

result = app_client.get_app(app)

```


### <a name="get_app__settings"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.get_app__settings") get_app__settings

> Get settings in an app

```python
def get_app__settings(self,
                          app,
                          _optional_query_parameters=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |
| _optional_query_parameters | ``` Optional ``` | Additional optional query parameters are supported by this method |



#### Example Usage

```python
app = 'app'
# key-value map for optional query parameters
optional_query_parameters = { }


result = app_client.get_app__settings(app, optional_query_parameters)

```


### <a name="get_app__mappings"></a>![Method: ](https://apidocs.io/img/method.png ".AppController.get_app__mappings") get_app__mappings

> Get an app's mappings.

```python
def get_app__mappings(self,
                          app)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| app |  ``` Required ```  | App name |



#### Example Usage

```python
app = 'app'

result = app_client.get_app__mappings(app)

```


[Back to List of Controllers](#list_of_controllers)



