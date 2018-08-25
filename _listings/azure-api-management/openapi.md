---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 1
info:
  title: ApiManagementClient
  description: use-these-rest-apis-for-performing-operations-on-user-entity-in-azure-api-management-deployment--the-user-entity-in-api-management-represents-the-developers-that-call-the-apis-of-the-products-to-which-they-are-subscribed-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/apis:
    get:
      summary: Apis ListByService
      description: Lists all APIs of the API Management service instance.
      operationId: Apis_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameapis-get
      parameters:
      - in: query
        name: $filter
        description: '| Field       | Supported operators    | Supported functions               ||-------------|------------------------|-----------------------------------||
          id          | ge, le, eq, ne, gt, lt | substringof, startswith, endswith
          || name        | ge, le, eq, ne, gt, lt | substringof, startswith, endswith
          || description | ge, le, eq, ne, gt, lt | substringof, startswith, endswith
          || serviceUrl  | ge, le, eq, ne, gt, lt | substringof, startswith, endswith
          || path        | ge, le, eq, ne, gt, lt | substringof, startswith, endswith
          |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - APIs
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/apis/{apiId}
  : get:
      summary: Apis Get
      description: Gets the details of the API specified by its identifier.
      operationId: Apis_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameapisapiid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - APIs
    put:
      summary: Apis CreateOrUpdate
      description: Creates new or updates existing specified API of the API Management
        service instance.
      operationId: Apis_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameapisapiid-put
      parameters:
      - in: header
        name: If-Match
        description: ETag of the Api Entity
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create or update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - APIs
    patch:
      summary: Apis Update
      description: Updates the specified API of the API Management service instance.
      operationId: Apis_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameapisapiid-patch
      parameters:
      - in: header
        name: If-Match
        description: ETag of the API entity
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: API Update Contract parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - APIs
    delete:
      summary: Apis Delete
      description: Deletes the specified API of the API Management service instance.
      operationId: Apis_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameapisapiid-delete
      parameters:
      - in: header
        name: If-Match
        description: ETag of the API Entity
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - APIs
---