# giti_terraform_jenkins

**Important**

```
Retrieving Admin Password for initial login:
User: admin
Password: to retrieve password use: sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```

**Plugins**

Always install suggested plug-ins + Make sure you have your desired plug-ins installed. 
```
**To install plugins from the dashboard**

Jenkins > Manage Plug-ins > Click on Available tab > Search for desired plug-in. 
```

**To add a worker node from the Dashboard On your master machine go to:**


```
Manage Jenkins > Manage Nodes > New Node
	a.	Enter Node Name
	b.	Select Permanent Agent 
	c.	Press OK. 
```	

**Fill out the following:**
```
	1.	Set a number of executors (one or more) as needed.
	2.	Set a Remote FS Root.
	3.	A home directory for the master on the agent machine. Most likely it will be /var/lib/jenkins
	       -For a Windows agent, use something like: "C:\Jenkins\"
	4.	Select the appropriate Usage setting:
	5.	For an additional worker: Utilize this node as much as possible
	6.	For specialized jobs: Leave this machine for tied jobs only
	7.	TODO: add steps for other methods.
	8.	Availability: Keep this agent online as much as possible
	9.	TODO: Add details for each option.
	10.	Press OK. 


Back to Dashboard you will see the worker node you just added. From there you can launch the node. 

```
