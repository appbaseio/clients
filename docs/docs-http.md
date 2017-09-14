# 

**`API Version:`** `1.0`

Appbase.io REST API



## Base URL

The base URL for this API is `https://scalr.api.appbase.io`



## Authentication
This API uses `basic authentication`.



### Authentication Parameters

The parameters required for authentication are listed below:

| Parameter | Description | Example | 
|-----------|-------------| ------- |
| username | username is the first part of the credentials (before ':') | `"TODO: Replace this"` |
| password | password is the second part of the credentials (after ':') | `"TODO: Replace this"` |





# <a name="api_reference"></a>API Reference

* [App](#app)

## <a name="app"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "App") App


### <a name="get_/:app"></a>![Endpoint: ](https://apidocs.io/img/method.png "GET /:app") GET /:app


**`GET`** `/{app}`

> Informational endpoint.


#### Base URL
This endpoint uses server ``.


#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| app | string |  ``` Required ```  | App name | `"app"` | 

#### Responses
**200** 


 *Example Body* (**dynamic**)


### <a name="get_/:app/_settings"></a>![Endpoint: ](https://apidocs.io/img/method.png "GET /:app/_settings") GET /:app/_settings


**`GET`** `/{app}/_settings`

> Get settings in an app




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| app | string |  ``` Required ```  | App name | `"app"` | 

#### Query Parameters
> Additional optional query parameters are allowed

#### Responses
**200** 


 *Example Body* (**dynamic**)


### <a name="get_/:app/_mappings"></a>![Endpoint: ](https://apidocs.io/img/method.png "GET /:app/_mappings") GET /:app/_mappings


**`GET`** `/{app}/_mappings`

> Get an app's mappings.




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| app | string |  ``` Required ```  | App name | `"app"` | 

#### Responses
**200** 


 *Example Body* (**dynamic**)


[Back to API Reference](#api_reference)

# <a name="models"></a> Models



