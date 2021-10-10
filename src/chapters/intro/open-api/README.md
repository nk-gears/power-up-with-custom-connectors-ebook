To have a readable swagger definition, create an API definition with the following structure:

SwaggerOpenAPI version (currently, only 2.0 is supported)
Information about the connector (title, description, status, contacts)
Host and supported schemes
Consumes/produces section
Paths (definitions of actions and triggers)
Definitions (Data types used in actions and triggers)
Parameters (Parameters that can be used across operations)



Open API - Quick Introduction

- Power Platform uses OpenAPI as the base protocol for building the conectors. Currently it supports the older version 2.0 aka swagger file.
- A Swagger file contains the definition of all the operations exposed by a API Service including the Input and Output Parameters along with Security like Basic Auth, OAuth or API Key based Authentications.

- A Typical Swagger file looks like this with some important property nodes like paths, definitions, parameters, responses etc.
 

- Request Schema

- Response Schema

```json
 {{#include ../../../snippets/open-api/path.json}}
```