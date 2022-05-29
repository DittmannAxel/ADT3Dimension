# Data connection to an IOT Hub

**First Step**:
- [Create an IOT Hub](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-create-through-portal)

**2nd Step**:<br>
The general How-To guide can be found [here](https://docs.microsoft.com/en-us/azure/digital-twins/how-to-ingest-iot-hub-data?tabs=cli) <br>
But wee need to adjust our settings based on the telemetry/naming from our ADT example.
So we need to adjust the function app from the example to change the naming, the object-IDs and the properties so that they could sent to the ADT instance.
The changed function app can be found here, but still needs to be fixed!
public async void Run([EventGridTrigger]EventGridEvent eventGridEvent, ILogger log) causes: 
https://docs.microsoft.com/en-us/azure/azure-functions/errors-diagnostics/sdk-rules/azf0001
Need to fix that first.
