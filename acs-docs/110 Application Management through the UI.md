# 110: Application Management through the UI
If you elected to configure a "jumpbox" you can create a VNC (for Linux jumpboxes) or RDP (Windows jumpboxes) connection to that machine and work with the UI from there. The first thing you need to do is configure an SSH tunnel to your cluster, see [108: Connecting to Orchestration Management Interfaces](108 Connecting to Orchestration REST API.md)

## VNC Connections for Linux Jumpboxes

If you elected to use a Linux Jumpbox then you will use VNC to connect to it. You will have needed to provide a tunnel to port 5901:

![](images/110/media/image1.png)

For more information on how to open a tunnel see [108: Connecting to Orchestration Management Interfaces](108 Connecting to Orchestration REST API.md).

Now install a VNC Client on your client (e.g. <http://www.realvnc.com/download/viewer/>)

Once installed open the client and connect as follows:

![](images/110/media/image2.png)

With the password of `password`.

![](images/110/media/image3.png)

You can now open a browser and view:

Now you can open a browser and visit:

-   Mesos: <http://master0:5050>

-   Marathon: <http://master0:8080>

-   Chronos: <http://master0:4400>

![](images/110/media/image4.png)

## Remote Desktop for Windows Jumpbox

To connect to a Windows Jumpbox you can find the RDP connection
details in the Azure Portal (see below for details). The admin
username is `azureuser`.

In the Azure portal navigate to your Jumpbox within your resource group:

![](images/110/media/image5.png)

![](images/110/media/image6.png)

Click the Connect button:

![](images/110/media/image7.png)

Optionally Save the file for easy access later. Open it now.

![](images/110/media/image8.png)

### Connect

Now you can connect using the password `azureuser`:

![](images/110/media/image9.png)

![](images/110/media/image10.png)

![](images/110/media/image11.png)

![](images/110/media/image12.png)

Now you can open a browser and visit:

-   Mesos: <http://master0:5050>

-   Marathon: <http://master0:8080>

-   Chronos: <http://master0:4400/>
