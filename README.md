# Data-Ingestion Into Azure-NoSQL

## Architecture Diagram 
![image](https://github.com/oigbokwe73/Data-Ingestion-IntoAzure-NoSQL/assets/15838780/ca75d3de-9b95-4a53-8780-d366f2cbb3e7)

## Video
[Low Code No Code](https://www.xenhey.com/api/GetFiling/614000248898)




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


  
## Products

|products|links|Comments|
|:----|:----|:----|
|Azure Getting Started |https://azure.microsoft.com/en-us/free/| Create free account + $200 in Credit|
|Azure Storage Explorer|https://azure.microsoft.com/en-us/features/storage-explorer/#features|useful view and query data in azure table storage|
|Postman|https://www.postman.com/downloads/|Postman supports the Web or Desktop Version|
|VsCode| https://visualstudio.microsoft.com/downloads/ |  Required extensions. Azure Functions, Azure Account
|VS Studio Community Edition |https://visualstudio.microsoft.com/downloads/| Recommended. Nice intergration with Azure. software is free.

## Low code No Code
1. **Accessibility**: LCNC platforms enable individuals without a deep technical background to develop applications. This democratizes the app development process, allowing a broader range of people to contribute.

2. **Speed**: With pre-built components and drag-and-drop interfaces, LCNC solutions can significantly reduce the time it takes to develop and deploy applications.

3. **Cost-Efficiency**: By reducing the need for specialized developers and speeding up the development process, businesses can save on development costs.

4. **Flexibility**: LCNC platforms often come with a wide range of customizable templates and components, allowing businesses to tailor applications to their specific needs.

5. **Scalability**: Many LCNC solutions are built on robust architectures that can scale with the growth of the business, ensuring that the applications remain performant as user numbers increase.

6. **Innovation**: By lowering the barriers to app development, LCNC platforms can foster innovation. Teams can quickly test new ideas and iterate based on feedback without committing significant resources.

7. **Maintenance**: LCNC platforms typically handle updates and maintenance, ensuring that applications remain up-to-date with the latest features and security patches.

8. **Integration**: Many LCNC platforms offer easy integration with other business tools and systems, allowing for seamless data flow and enhanced functionality.

9. **Consistency**: With standardized components and templates, businesses can ensure a consistent user experience across different applications.

10. **Empowerment**: LCNC solutions empower non-technical team members, such as business analysts and managers, to take a more active role in the digital transformation of their organizations.

In summary, Low Code No Code solutions offer a way for businesses to rapidly develop and deploy applications, reduce costs, and foster innovation, all while ensuring scalability and consistency. They represent a shift in how applications are developed, placing more power in the hands of end-users and reducing reliance on traditional development processes.
## Contact
  
For questions related to this project, can be reached via email :- support@xenhey.com
