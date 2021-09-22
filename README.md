# Mule-Salesforce-BulkAPI2.0
Invoking Salesforce Bulk API 2.0 from MuleSoft

As long as it is a simple update to sobject and no business logic is needed, Bulk API is the best way to insert data into Salesforce from MuleSoft without hitting governor limits. The onus is on Salesforce to keep track of all the job status.

Mule will receive the below response from Salesforce, as you can see the state is InProgress, which does not tell anything (success/failure) about the job status.

Ref: https://mulesy.com/process-records-using-salesforce-bulk-api-2-0/

response: 
{  
  "lineEnding": "CRLF",  
  "numberRecordsFailed": 0,  
  "externalIdFieldName": "External_ID__c",  
  "numberRecordsProcessed": 0,  
  "errorMessage": null,  
  "systemModstamp": "2021-09-22T14:27:04.000+0000",  
  "apiActiveProcessingTime": 0,  
  "concurrencyMode": "Parallel",  
  "retries": 0,  
  "apexProcessingTime": 0,  
  "createdDate": "2021-09-22T14:27:04.000+0000",  
  "apiVersion": "52.0",  
  "id": "7505G00000ijiDFQAY",  
  "state": "InProgress",  
  "jobType": "V2Ingest",  
  "totalProcessingTime": 0,  
  "contentType": "CSV",  
  "operation": "upsert",  
  "createdById": "005f4000003JwANAA0",  
  "object": "score__c",  
  "columnDelimiter": "COMMA"  
} 
