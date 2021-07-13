# adf-assignment-1

FOLDER - 1 
_____________
In this assignment, I have played around with some services of Azure such as Azure Data Factory and Azure Blob storage

Azure Data Factory (ADF) is a data processing platform where we can extract, load and transform or extract, transform and then load the data into a particular table/file as per the need. 

Here, to try the trigger, I have implemented a New trigger named "RunWhenFileDrops" which triggers the movement of .csv file from a blob named Input to another blob named Output. 

In the trigger, I have put the blob location named Trigger where when a file drops, it triggers the movement. 

I have faced an issue where the Microsoft.EventGrid was not registered in the subscription. To solve that, I went to the Subscription and then under Settings we go to Resource Providers and then type "event" in the search box, and then register Microsoft.EventGrid. 

After that we publish the changes made in the trigger so that the changes are saved and then we try to run the trigger. The pipeline works fine. 

____________________
