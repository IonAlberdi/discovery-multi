##Discovery-Multi Hello World

This HelloWorld shows the discoveryForAgentContext and applicationContext librarys developed for the [MediaScape project](http://mediascapeproject.eu/) in action. 

## Navigation
[Installation][] | [Prerequisite][] | [Deployment][]  | [Run][]

###Installation
####Prerequisite
* Install git
* Install node.js and npm
* Install mongodb
* Start mongodb

####Deployment
Next to this file you will find a script called `deploy.sh`.  
This script will:
1. clone the git and install everything in a folder called `deploy` relative to the file itsself
2. copy the [server](https://github.com/mediascape/application-context/tree/master/Server) and [Application Context API inluding Agent Context](../API), [Discovery For Agent Context API](../API) and [Discovery API](https://github.com/mediascape/discovery-self/tree/master/API) including this HelloWorld sample
3. install all needed dependencies for the backend and start a small setup-script to configure it.

*Please dont execute it inside the git folder. Best practice is to download just the the `.sh` file and execute.*

### run
After everything is set up, and the node.js server is started, you can access the demo using the url (depending on your setup): 
```
    http://localhost:8080/index.html
```
When the page is loaded, it should show you the detected components and capabilities of your current device.
Starting another Browser with the same URL this data will be shared via the Agent Context between all sessions.


Any time later you can start the node.js server via:

```bash
node index.js
```

[Installation]: #installation
[Prerequisite]: #prerequisite
[Deployment]: #deployment
[Run]: #run
