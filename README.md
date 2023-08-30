# Data-Ingestion Into Azure-NoSQL

## Architecture Diagram 
![image](https://github.com/oigbokwe73/Data-Ingestion-IntoAzure-NoSQL/assets/15838780/ca75d3de-9b95-4a53-8780-d366f2cbb3e7)






## Appplication Setting 

|Key|Value | Comment|
|:----|:----|:----|
|AzureWebJobsStorage|[CONNECTION STRING]|RECOMMENDATION :  store in AzureKey Vault.|
|ConfigurationPath| [CONFIGURATION FOLDER PATH] |Folder is optional
|ApiKeyName|[API KEY NAME]|Will be passed in the header  :  the file name of the config.
|AppName| [APPLICATION NAME]| This is the name of the Function App. Used in log analytics|
|StorageAcctName|[STORAGE ACCOUNT NAME]|Example  "AzureWebJobsStorage"|

## Function App  Configuration 

> **Note:** The **Configuration** is located in the  FunctionApp  in a **Config** Folder.

|FileName|Description|
|:----|:----|
|43EFE991E8614CFB9EDECF1B0FDED37B.json| Create a single record in  NOSQL Database.|
|43EFE991E8614CFB9EDECF1B0FDED37C.json| Search NOSQL Database for result set|
|43EFE991E8614CFB9EDECF1B0FDED37D.json| Upload JSON File into No SQL DB|
|43EFE991E8614CFB9EDECF1B0FDED37A.json| Upload CSV file|
|43EFE991E8614CFB9EDECF1B0FDED37E.json| Delete Record from NoSQLData|
|43EFE991E8614CFB9EDECF1B0FDED37F.json| Update record in NoSQL database|


## How to install ACI for SFTP
https://docs.microsoft.com/en-us/samples/azure-samples/sftp-creation-template/sftp-on-azure


  
## Products

|products|links|Comments|
|:----|:----|:----|
|Azure Getting Started |https://azure.microsoft.com/en-us/free/| Create free account + $200 in Credit|
|Azure Storage Explorer|https://azure.microsoft.com/en-us/features/storage-explorer/#features|useful view and query data in azure table storage|
|Postman|https://www.postman.com/downloads/|Postman supports the Web or Desktop Version|
|VsCode| https://visualstudio.microsoft.com/downloads/ |  Required extensions. Azure Functions, Azure Account
|VS Studio Community Edition |https://visualstudio.microsoft.com/downloads/| Recommended. Nice intergration with Azure. software is free.


## Contact
  
For questions related to this project, can be reached via email :- support@xenhey.com
