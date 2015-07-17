# Discovery-Multi API

## Navigation
[Overview][] | [Architecture][] | [API][]

## Overview
[Top][]

Creates some components based on [Implementing Custom Components](https://github.com/mediascape/application-context/tree/master/API#implementing-custom-components) and using the [Discovery API](https://github.com/mediascape/discovery-self/tree/master/API).

## Architecture
[Top][]

In the following schema can be seen the integration of Discovery-Self and Application Context:

![alt text](./mediascape_discovery_multi.png "MediaScape - Agent and Application Context")

## API
[Top][]

Those are the agents that Discovery-Multi API discovers and encapsulates into Custom Components:

* UPNP

	Calls mediascape.discovery.isPresent function to detect the presence of the upnp agent, if the agent exists, the system sets the upnp status as supported, unless it will be set as unsupported. Then it will initialize upnp value calling to mediascape.discovery.getDevices and returning the list of ids of the services available to consume by upnp.

* Bluetooth

	Calls mediascape.discovery.isPresent function to detect the presence of the bluetooth agent, if the agent exists, the system sets the bluetooth status as supported, unless it will be set as unsupported. Then it will initialize bluetooth value calling to mediascape.discovery.getDevices and returning the list of ids of the devices available to connect by bluetooth.

* NamedWebSockets

	Calls mediascape.discovery.isPresent function to detect the presence of the NamedWebSockets agent, if the agent exists, the system sets the namedwebsockets status as supported, unless it will be set as unsupported. Then it will initialize namedwebsockets value calling to mediascape.discovery.getDevices and returning the list of ids of the devices connected to namedwebsockets "mediascape".

* Screen Size

	Calls mediascape.discovery.isPresent function to detect the presence of the screen size agent, if the agent exists, the system sets the screenSize status as supported, unless it will be set as unsupported. Then it will initialize screenSize value calling to mediascape.discovery.getExtra and returning the size of the screen of the device and will define on and off functions to subscribe to an event. This event will return the changes hapened on the size of the screen.

* Language

	Calls mediascape.discovery.isPresent function to detect the presence of the language agent, if the agent exists, the system sets the language status as supported, unless it will be set as unsupported. Then it will initialize language value calling to mediascape.discovery.getExtra and returning the language of the device.

* Platform

 	Calls to navigator.platform function to detect the presence of the platform agent, if the agent exists, the system sets the platform status as supported, unless it will be set as unsupported. Then it will initialize platform value calling to navigator.platform and returning the platform of the device.

* NavigatorProduct

	Calls to navigator.product function to detect the presence of the product agent, if the agent exists, the system sets the navigatorProduct status as supported, unless it will be set as unsupported. Then it will initialize navigatorProduct value calling to navigator.platform and returning the the engine (product) name of the device browser.
	
* On Line

	Calls to navigator.onLine function to detect the presence of the onLine agent, if the agent exists, the system sets the onLine status as supported, unless it will be set as unsupported. Then it will initialize onLine value calling to navigator.onLine and returning if the device is connected.

* Device Type

	Calls mediascape.discovery.isPresent function to detect the presence of the deviceType agent, if the agent exists, the system sets the deviceType status as supported, unless it will be set as unsupported. Then it will initialize deviceType value calling to mediascape.discovery.getExtra and  returning the type of the device.

* User Proximity

	Calls mediascape.discovery.isPresent function to detect the presence of the geolocation agent, if the agent exists, the system sets the geolocation status as supported, unless it will be set as unsupported.Then it will initialize geolocation value calling to mediascape.discovery.getExtra and returning the state of the geolocation senson of the device and will define on and off functions to subscribe to an event. This event will return the changes hapened on the geolocation sensor.

* User Proximity

	Calls mediascape.discovery.isPresent function to detect the presence of the user proximity agent, if the agent exists, the system sets the userProximity status as supported, unless it will be set as unsupported.Then it will initialize userProximity value calling to mediascape.discovery.getExtra and returning the state of the user proximity senson of the device and will define on and off functions to subscribe to an event. This event will return the changes hapened on the user proximity sensor.

* Device Proximity

	Calls mediascape.discovery.isPresent function to detect the presence of the device proximity agent, if the agent exists, the system sets the deviceProximity status as supported, unless it will be set as unsupported. Then it will initialize deviceProximity value calling to mediascape.discovery.getExtra and returning the state of the device proximity senson of the device and will define on and off functions to subscribe to an event. This event will return the changes hapened on the device proximity sensor.

* Touch Screen

	Calls mediascape.discovery.isPresent function to detect the presence of the touchScreen agent, if the agent exists, the system sets the touchScreen status as support, unless it will be set as unsupported.

* Vibration

	Calls mediascape.discovery.isPresent function to detect the presence of the vibration agent, if the agent exists, the system sets the vibration status as maybe, unless it will be set as unsupported.
		
* Screen Orientation

	Calls mediascape.discovery.isPresent function to detect the presence of the screen orientation agent, if the agent exists, the system sets the orientation status as supported, unless it will be set as unsupported. Then it will initialize orientation value calling to mediascape.discovery.getExtra and returning the orientation of the device and will define on and off functions to subscribe to the events. This events will return the changes hapened on orientation.

* Connection

	Calls mediascape.discovery.isPresent function to detect the presence of the connection agent, if the agent exists, the system sets the connection status as supported, unless it will be set as unsupported. Then it will initialize connection value calling to mediascape.discovery.getExtra and returning the type of the connection of the device and will define on and off functions to subscribe to a event. This events will return the changes hapened on connection type.

* Audio

	Calls mediascape.discovery.isPresent function to detect the presence of the audio agent, if the agent exists, the system sets the video status as supported, unless it will be set as unsupported. Then it will initialize audio value calling to mediascape.discovery.getExtra and returning the number of audio elements of the device.

* Camera

	Calls mediascape.discovery.isPresent function to detect the presence of the camera agent,if the agent exists, the system sets the camera status as supported, unless it will be set as unsupported. Then it will initialize video value calling to mediascape.discovery.getExtra and returning the number of cameras of the device.

* Battery
	
	Calls mediascape.discovery.isPresent function to detect the presence of th battery agent, if the agent exists, the system sets the battery status as supported, unless it is set as unsupported. Then it will initialize battery value calling to mediascape.discovery.getExtra and will define on and off functions to subscribe to different events. This events will return the changes hapened on battery level changes, on battery charging changes on battery discharging time changes.


[Top]: #navigation
[Overview]: #overview
[Architecture]: #architecture
[API]: #api
