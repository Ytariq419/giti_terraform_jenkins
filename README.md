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
To install plugins from the dashboard

Jenkins > Manage Plug-ins > Click on Available tab > Search for desired plug-in. 
```

To add a worker node from the Dashboard:

On your master machine go to Manage Jenkins > Manage Nodes.

New Node
	a.	Enter Node Name
	b.	Select Permanent Agent 
	c.	Press OK. 
Fill out the following:
	a.	Set a number of executors 
	i.	(one or more) as needed.
	b.	Set a Remote FS Root
	i.	a home directory for the master on the agent machine. Most likely it will be /var/lib/jenkins
	ii.	For a Windows agent, use something like: "C:\Jenkins\"
	c.	Select the appropriate Usage setting:
	i.	For an additional worker: Utilize this node as much as possible
	ii.	For specialized jobs: Leave this machine for tied jobs only
	d.	Launch Method:
	i.	An easy way to control a Windows agent is by using Launch agent via Java Web Start  (Recommended for Windows)
	ii.	TODO: add steps for other methods.
	e.	Availability 
	i.	Keep this agent online as much as possible
	ii.	TODO: add details for each option.
	f.	Press OK. 
Back to Dashboard you will see the worker node you just added. From there you can launch the node. 
