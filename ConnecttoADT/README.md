# External data connection to ADT

## Connection via REST API
**Postman**
A short introduction on how to setup the authentification and the Postman connection:
https://docs.microsoft.com/en-us/azure/digital-twins/how-to-use-postman?tabs=data-plane

And the link to the Git repo, how to find the collection.
https://github.com/microsoft/azure-digital-twins-postman-samples


## Data connection to an IOT Hub

**First Step**:
- [Create an IOT Hub](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-create-through-portal)

**2nd Step**:<br>
The general How-To guide can be found [here](https://docs.microsoft.com/en-us/azure/digital-twins/how-to-ingest-iot-hub-data?tabs=cli) <br>
But wee need to adjust our settings based on the telemetry/naming from our ADT example.
So we need to adjust the function app from the example to change the naming, the object-IDs and the properties so that they could sent to the ADT instance.
The original example contains:
public async void Run([EventGridTrigger]EventGridEvent eventGridEvent, ILogger log) causes: 
https://docs.microsoft.com/en-us/azure/azure-functions/errors-diagnostics/sdk-rules/azf0001 <br>
But is is fixed in the lab:
https://microsoftlearning.github.io/AZ-220-Microsoft-Azure-IoT-Developer/Instructions/Labs/LAB_AK_19-azure-digital-twins.html

So I will provide here only the code changes for this windturbine example.

