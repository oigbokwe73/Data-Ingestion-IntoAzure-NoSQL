# Data-Ingestion Into Azure-NoSQL

## Architecture Diagram 
![image](![image](https://github.com/oigbokwe73/Data-Ingestion-IntoAzure-NoSQL/assets/15838780/6d8b0486-3533-465d-8355-e2e26967b664)
)



## Appplication Setting 

|Key|Value | Comment|
|:----|:----|:----|
|AzureWebJobsStorage|[CONNECTION STRING]|RECOMMENDATION :  store in AzureKey Vault.|
|ConfigurationPath| [CONFIGURATION FOLDER PATH] |Folder is optional
|ApiKeyName|[API KEY NAME]|Will be passed in the header  :  the file name of the config.
|AppName| [APPLICATION NAME]| This is the name of the Function App. Used in log analytics|
|StorageAcctName|[STORAGE ACCOUNT NAME]|Example  "AzureWebJobsStorage"|
|TimerInterval|[TIMER_INTERVAL]|Example  "0 */1 * * * *" 1 MIN|

## Function App  Configuration 

> **Note:** The **Configuration** is located in the  FunctionApp  in a **Config** Folder.

|FileName|Description|
|:----|:----|
|43EFE991E8614CFB9EDECF1B0FDED37A.json| Upload CSV file|
|43EFE991E8614CFB9EDECF1B0FDED37B.json| Send JSON Post Request into Azure NOSQL Database.|
|43EFE991E8614CFB9EDECF1B0FDED37C.json| Search NOSQL Database for result set. Custom Mapping to result set.|
|43EFE991E8614CFB9EDECF1B0FDED37D.json| Upload and shard into batch sizes.|
|43EFE991E8614CFB9EDECF1B0FDED37E.json| Event triggered when file is written to container|
|43EFE991E8614CFB9EDECF1B0FDED37F.json| Copy File(s) from File share to contrainer. File is droppoed using SFTP|


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

## bug
  
if the  csv has "," in the payload will throw  a "column header error". Only use CSV's without  Commas(",") in the  
  
  
  ## Contact
  
For questions related to this project, can be reached via email :- support@xenhey.com
