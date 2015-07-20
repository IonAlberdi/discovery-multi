#Discovery-Multi

In this folder you will find the Discovery For Agent Context. It means mechanism to propagate the Discovery features across different devices on top of the Aplication Context developed for [MediaScape project](http://mediascapeproject.eu/).

## Navigation
[Goals][] | [Structure][] | [Authors][] | [License][]

### Goals
[Top][]

MediaScape targets applications that provide shared experiences across multiple devices.

In this context, to ease distributed application decisions, different devices running an application must provide shared awareness of their capabilities and features.

Discovery-Multi integrates Agent Context and Discovery-Self to provide information about the current agent, it’s capabilities and events (as well as sensor management) based in Discovering API published into Discovery-Self.

Discovery propagation through the Aplication Context includes two developments:
* Discovery API:
This library build awareness about the device features and the available devices ready to be connected to each application instance.
https://github.com/mediascape/discovery-self
* Application Context:
The Application context includes the Agent context that focus on information related to an agent, it’s capabilities and provides events with updates 
https://github.com/mediascape/application-context


### Structure
[Top][]

The generic structure of each WP repository is:

  * API: The JavaScript API.
  * helloworld: minimal sample code.

### Authors
[Top][]

- Ion Alberdi (ialberdi@vicomtech.org)
- Angel Martin (amartin@vicomtech.org)

### License
[Top][]

Copyright 2015 Vicomtech.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

[Top]: #navigation
[Goals]: #goals
[Structure]: #structure
[Authors]: #authors
[License]: #license
