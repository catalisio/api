# Catalisio API
## Overview
### Authentification
Each request must have the header `X-Auth-Token: <your_token>`.

A token is an authentification for one site.
### Response
The response is formatted in JSON. 
```
{
    "body" : {<JSON>},
    "elapsedTime" : <double>,
    "hasError" : <boolean>,
    "errorDetail" : <string>,
    "errorType" : <integer>
}
```
* `body` : body of the response
* `elaspedTime` : number of seconds for the processing of the response
* `hasError` : indicates if the response is an error or not
* `errorDetail` : if the response is an error, get the details
* `errorType` : http status code

If the response is an error, the http status code is different than `200`.
