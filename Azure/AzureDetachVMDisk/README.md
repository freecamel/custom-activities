## AzureDetachVMDisk - Activity to detach Data Disk from a Virtual Machine.

Remark - The portal needs to be configured first. https://portal.azure.com

##### DLL's to reference
Microsoft.Azure.Management.Compute.Fluent.dll
Microsoft.Azure.Management.Fluent.dll
Microsoft.Azure.Management.ResourceManager.Fluent.dll
Microsoft.Azure.Management.Network.Fluent.dll
Microsoft.Azure.Management.Sql.Fluent.dll
Microsoft.Rest.ClientRuntime.dll
Microsoft.Rest.ClientRuntime.Azure.dll
System.Net.Http.dll
Newtonsoft.Json.dll

##### Libraries to import
using Microsoft.Azure.Management.Compute.Fluent;
using Microsoft.Azure.Management.Fluent;
using Microsoft.Azure.Management.ResourceManager.Fluent;
using Microsoft.Azure.Management.ResourceManager.Fluent.Core


You'd need to store the API specific information from the portal.

ApplicationId
TenantId
Secret

### Mandatory fields when detaching a data disk from VM:

**subscriptionId**		- The azure portal subscription Id (Free Trial/Premium)

**vmName**				- Virtual Machine name where to detach the disk.

**diskName**			- The name of the disk to detach
