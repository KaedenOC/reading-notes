# CRUD

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

## Status Codes

- **100's** - Informational. Indicates that the request was received and the process is continuing.

- **200's** - Success. Indicates that the request was successful.

- **300's** - Redirection. Indicates that further action is needed to complete the request.

- **400's** - Client Error. Indicates that there was an error on the client side.

- **500's** - Server Error. Indicates that there was an error on the server side.

- **202** - That the request has been accepted for processing, but the processing has not been completed yet.

- **308** - That the resource has been moved permanently to a new location and the client should update its URL.

- If an update didn't return data to a client, you would use the status code **204** No Content.

- You would use the status code **410** Gone, if a resource used to exist but no longer does.

- **403** -  'Forbidden' - The client does not have permission to access the requested resource.

