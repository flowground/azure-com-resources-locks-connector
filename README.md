# ![LOGO](logo.png) ManagementLockClient **flow**ground Connector

## Description

A generated **flow**ground connector for the ManagementLockClient API (version 2016-09-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/resources-locks/2016-09-01/swagger.json<br/>
Generated at: 2019-05-07T17:38:46+03:00

## API Description

Azure resources can be locked to prevent other users in your organization from deleting or modifying resources.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all of the available Microsoft.Authorization REST API operations.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - The API version to use for the operation.

### Gets all the management locks for a subscription.

*Tags:* `ManagementLocks`

#### Input Parameters
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes the management lock at the subscription level.

> To delete management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.

*Tags:* `ManagementLocks`

#### Input Parameters
* `lockName` - _required_ - The name of lock to delete.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets a management lock at the subscription level.

*Tags:* `ManagementLocks`

#### Input Parameters
* `lockName` - _required_ - The name of the lock to get.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Creates or updates a management lock at the subscription level.

> When you apply a lock at a parent scope, all child resources inherit the same lock. To create management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.

*Tags:* `ManagementLocks`

#### Input Parameters
* `lockName` - _required_ - The name of lock. The lock name can be a maximum of 260 characters. It cannot contain <, > %, &, :, \, ?, /, or any control characters.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets all the management locks for a resource group.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group containing the locks to get.
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes a management lock at the resource group level.

> To delete management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group containing the lock.
* `lockName` - _required_ - The name of lock to delete.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets a management lock at the resource group level.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the locked resource group.
* `lockName` - _required_ - The name of the lock to get.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Creates or updates a management lock at the resource group level.

> When you apply a lock at a parent scope, all child resources inherit the same lock. To create management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group to lock.
* `lockName` - _required_ - The lock name. The lock name can be a maximum of 260 characters. It cannot contain <, > %, &, :, \, ?, /, or any control characters.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Gets all the management locks for a resource or any level below resource.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group containing the locked resource. The name is case insensitive.
* `resourceProviderNamespace` - _required_ - The namespace of the resource provider.
* `parentResourcePath` - _required_ - The parent resource identity.
* `resourceType` - _required_ - The resource type of the locked resource.
* `resourceName` - _required_ - The name of the locked resource.
* `$filter` - _optional_ - The filter to apply on the operation.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Deletes the management lock of a resource or any level below the resource.

> To delete management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group containing the resource with the lock to delete. 
* `resourceProviderNamespace` - _required_ - The resource provider namespace of the resource with the lock to delete.
* `parentResourcePath` - _required_ - The parent resource identity.
* `resourceType` - _required_ - The resource type of the resource with the lock to delete.
* `resourceName` - _required_ - The name of the resource with the lock to delete.
* `lockName` - _required_ - The name of the lock to delete.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Get the management lock of a resource or any level below resource.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group. 
* `resourceProviderNamespace` - _required_ - The namespace of the resource provider.
* `parentResourcePath` - _required_ - An extra path parameter needed in some services, like SQL Databases.
* `resourceType` - _required_ - The type of the resource.
* `resourceName` - _required_ - The name of the resource.
* `lockName` - _required_ - The name of lock.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Creates or updates a management lock at the resource level or any level below the resource.

> When you apply a lock at a parent scope, all child resources inherit the same lock. To create management locks, you must have access to Microsoft.Authorization/* or Microsoft.Authorization/locks/* actions. Of the built-in roles, only Owner and User Access Administrator are granted those actions.

*Tags:* `ManagementLocks`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group containing the resource to lock. 
* `resourceProviderNamespace` - _required_ - The resource provider namespace of the resource to lock.
* `parentResourcePath` - _required_ - The parent resource identity.
* `resourceType` - _required_ - The resource type of the resource to lock.
* `resourceName` - _required_ - The name of the resource to lock.
* `lockName` - _required_ - The name of lock. The lock name can be a maximum of 260 characters. It cannot contain <, > %, &, :, \, ?, /, or any control characters.
* `api-version` - _required_ - The API version to use for the operation.
* `subscriptionId` - _required_ - The ID of the target subscription.

### Delete a management lock by scope.

*Tags:* `ManagementLocks`

#### Input Parameters
* `scope` - _required_ - The scope for the lock. 
* `lockName` - _required_ - The name of lock.
* `api-version` - _required_ - The API version to use for the operation.

### Get a management lock by scope.

*Tags:* `ManagementLocks`

#### Input Parameters
* `scope` - _required_ - The scope for the lock. 
* `lockName` - _required_ - The name of lock.
* `api-version` - _required_ - The API version to use for the operation.

### Create or update a management lock by scope.

*Tags:* `ManagementLocks`

#### Input Parameters
* `scope` - _required_ - The scope for the lock. When providing a scope for the assignment, use '/subscriptions/{subscriptionId}' for subscriptions, '/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}' for resource groups, and '/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{parentResourcePathIfPresent}/{resourceType}/{resourceName}' for resources.
* `lockName` - _required_ - The name of lock.
* `api-version` - _required_ - The API version to use for the operation.

## License

**flow**ground :- Telekom iPaaS / azure-com-resources-locks-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
