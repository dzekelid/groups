---
swagger: "2.0"
x-collection-name: Azure IoT Hub
x-complete: 1
info:
  title: iotHubClient
  description: use-this-api-to-manage-the-iot-hubs-in-your-subscription-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/IotHubs/{resourceName}/eventHubEndpoints/{eventHubEndpointName}/ConsumerGroups
  : get:
      summary: Iot Hub Resource List Event Hub Consumer Groups
      description: Get a list of the consumer groups in the Event Hub-compatible device-to-cloud
        endpoint in an IoT hub.
      operationId: IotHubResource_ListEventHubConsumerGroups
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devicesiothubsresourcenameeventhubendpointseventhubendpointnameconsumergroups-get
      parameters:
      - in: path
        name: eventHubEndpointName
        description: The name of the Event Hub-compatible endpoint
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the IoT hub
      - in: path
        name: resourceName
        description: The name of the IoT hub
      responses:
        200:
          description: OK
      tags:
      - Iot Hub Resource Event Hub Consumer Groups
---