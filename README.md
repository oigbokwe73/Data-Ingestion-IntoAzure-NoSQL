# Data-Ingestion IntoAzure-NoSQL

## Architecture Diagram 
![image](https://user-images.githubusercontent.com/15838780/159803055-8ee721bf-ca24-4bfb-92e9-aa8c4d51af20.png)


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
|43EFE991E8614CFB9EDECF1B0FDED37A.json| Upload CSV file|
|43EFE991E8614CFB9EDECF1B0FDED37B.json| Send JSON Post Request into Azure NOSQL Database.|
|43EFE991E8614CFB9EDECF1B0FDED37C.json| Search NOSQL Database for result set. Custom Mapping to result set.|
|43EFE991E8614CFB9EDECF1B0FDED37D.json| Upload and shard into batch sizes.|
|43EFE991E8614CFB9EDECF1B0FDED37E.json| Event triggered when file is written to container|


## Upload Configuration to Storage
Go to created storage Account.. Click On "Blob Service" 
![image](https://user-images.githubusercontent.com/15838780/147958072-4a6058d2-d320-44a0-9d11-58449d527cd3.png)

Click on **"Container"**
![image](https://user-images.githubusercontent.com/15838780/147958201-71df0f21-e4e8-46c0-93be-728f1dbc2a43.png)
![image](https://user-images.githubusercontent.com/15838780/147963170-1a2f2a64-7ba2-44ce-9f5d-30d490529711.png)
Upload the selected files from the "**Config**" folder in your project

  
  ## Products

|products|links|Comments|
|:----|:----|:----|
|Azure Getting Started |https://azure.microsoft.com/en-us/free/| Create free account + $200 in Credit|
|Azure Storage Explorer|https://azure.microsoft.com/en-us/features/storage-explorer/#features|useful view and query data in azure table storage|
|Postman|https://www.postman.com/downloads/|Postman supports the Web or Desktop Version|
|VsCode| https://visualstudio.microsoft.com/downloads/ |  Required extensions. Azure Functions, Azure Account
|VS Studio Community Edition |https://visualstudio.microsoft.com/downloads/| Recommended. Nice intergration with Azure. software is free.

## bug
  
if the  csv has "," in the payload will throw  a "column header error". Only use CSV's without  Commas(",") in the  
  
  
  ## Contact
  
For questions related to this project, can be reached via email :- support@xenhey.com

