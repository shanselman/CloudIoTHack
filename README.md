# Cloud City IoT Hack #

---

## Overview ##

This repo contains content for the Cloud City IoT Hack, an event that provides developers with a hands-on introduction to some of the very best features Microsoft Azure has to offer, including [IoT Hubs](https://azure.microsoft.com/services/iot-hub/), [Event Hubs](https://azure.microsoft.com/services/event-hubs/), [Azure Functions](https://azure.microsoft.com/services/functions/), [Stream Analytics](https://azure.microsoft.com/services/stream-analytics/), and [Cognitive Services](https://azure.microsoft.com/services/cognitive-services/). Four hands-on labs are found in folders named HOL 1, HOL 2, HOL 3, and HOL 4. Here's a synopsis of those labs:

- HOL 1 - Attendees create an Azure IoT Hub and program an [MXCHIP]([MXChip](https://microsoft.github.io/azure-iot-developer-kit/)) to send accelerometer data to it.
- HOL 2 - Attendees create an Azure Event Hub and deploy an Azure Function that transforms accelerometer data input to the IoT Hub into "flight data" denoting the disposition on an airplane and transmits it to the Event Hub. Then they connect a UWP client app to the Event Hub and use their MXChip to fly a simulated airplane.
- HOL 3 - The instructor creates a pair of Event Hubs and deploys a Stream Analytics job that analyzes all the air traffic in the room for aircraft that are within two miles of aech another. He or she also deploys a UWP app that shows all the air traffic.
- HOL 4 - Attendees modify the Azure Function they deployed in Lab 2 to transmit flight data to the input hub used by Stream Analytics. They also connect the client app to the Stream Analytics output and modify the app to transmit warning messages back to the MXChip when their aircraft are within two miles of another.

The repo also has three folders containing source code used in the labs:

- FlySim - A Visual Studio 2017 solution containing the client app that attendees use to fly simulated airplanes
- FlySimEmbedded - The code attendees upload to the MXChip to program it to send accelerometer data to an IoT Hub 
- AirTrafficSim - A Visual Studio 2017 solution containing the air-traffic control (ATC) app that shows all the airplanes in flight and highlights those that are within two miles of each other.

For an overview of the end-to-end solution featured in the event, see the introduction to HOL 1.

## Contributing ##

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
