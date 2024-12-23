# Anatomy of a URL
Universal Resource Location

*https://*                        **linkedin\.com/learning**

***Protocol declaration*   URN: Unifrom Resource Name**

**linkedin.com** -> Host :443 - Connection port (usually hidden)
**learning ...** -> Resource path

# HTTP Methods

GET: get the specified resource, if available
```mermaid
flowchart TD
GET --Success --> 200_OK
GET --Failure --> 404_NotFound
GET --Failure --> 405_NotAllowed
GET --Failure --> 403_Forbidden
```

POST: create anew resource and add it to a collection
```mermaid
flowchart TD
POST --Success --> 201_Created
POST --Failure --> 401_Unauthorized
POST --Failure --> 409_Conflict
POST --Failure --> 404_NotFound
```

PUT: update an existing singleton resource based on ID
```mermaid
flowchart TD
PUT --Success --> 200_OK
PUT --Failure --> 204_NoContent
PUT --Failure --> 405_MethodNotAllowed
PUT --Failure --> 404_NotFound
```

PATCH: modify an existing singleton resource based on ID
```mermaid
flowchart TD
PATCH --Success --> 200_OK
PATCH --Failure --> 204_NoContent
PATCH --Failure --> 405_MethodNotAllowed
PATCH --Failure --> 404_NotFound
```

DELETE: delete a singleton resource based on ID
```mermaid
flowchart TD
DELETE --Success --> 200_OK
DELETE --Failure --> 401_Unauthorized
DELETE --Failure --> 405_MethodNotAllowed
DELETE --Failure --> 404_NotFound
```

HEAD: get just the response headers from the resource
```mermaid
flowchart TD
HEAD --Success --> 200_OK
HEAD --Failure --> 404_NotFound
```

OPTIONS: get the options available from this resource
```mermaid
flowchart TD
OPTIONS --Success --> 200_OK
```

TRACE: create a loopback for the request message
```mermaid
flowchart TD
TRACE --Success --> 200_OK
```

# HTTP status messages

| Status Code | Grouping     |
| ----------- | ------------ |
| 1xx         | Information  |
| 2xx         | Success      |
| 3xx         | Redirection  |
| 4xx         | Client error |
| 5xx         | Server error |
