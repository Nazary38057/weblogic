# Prepare Setup

## Introduction

This lab will show you how to configure Outgoing Provider setup the Archiver, a Java applet, on the Source WebCenter Content Instance.


**Estimated Lab Time**: *TBD*

### Objectives

- Setup the Archiver on Source WebCenter Content Instance


## Task 2: Setup Archiver on Target WebCenter Content Instance
### **2.1 Sign in to WebCenter Content Administration UI**

Complete the following steps to sign in to the Oracle Cloud Infrastructure console.

  1. Go to the Target WebCenter Content Administration UI. For example `https://source-wcc.mydomain.com/cs` 
  ![Administration UI Login](images/01.01.source-archive-setup.AdminLogin.png "Administration UI Login")

  2. Enter your WebCenter Content Administrator Cloud account login credentials
  ![OCI Login](images/01.02.target-archive-setup.TenancyLogin.png "OCI Login")

  3. Click on "Sign In" button 
  ![Administration UI](images/01.03.target-archive-setup.WebCenter_Admin_UI.png "Administration UI")



### **2.2 Configure Replication Provider on the Source WebCenter Content Instance**

1. In WebCenter Content UI, navigate to *Administration* --> *Providers* and click on *Add* button of *outgoing* Provider Type
![Providers](images/2.2.01.target-provider-add.png " ")

2. On *Edit Outgoing Socket Provider* page populate required fields 
- **Provider Name** : Name of your choosing 
- **Provider Description** : Provider Description
- **Server Host Name** : FQDN Host name of the Target WebCenter Content System
- **Server Port** : Target WebCenter Content System port, usually 4444
- **Instance Name** : Instance name obtained from previous lab
- **Relative Web Root** : /cs/ 
![Providers](images/2.2.02.target-provider-add.png "Providers")

Click *Add* button

3. Verify newly created provider listed in *Providers* table
![Providers](images/2.2.03.target-providers-listed.png " ")
NOTE that *Connection State* for the Provider we added, is *new Requires Restart*

4. Restart WebCenter Content UCM managed servers 

5. Refresh WebCenter Content UI *Administration* --> *Providers* page and verify new Outgoing provider *Connection State* is *good*
  ![Providers](images/2.2.04.target-providers-good.png " ")

6. Test Outgoing Provider by clicking on *Test* link
  ![Providers](images/2.2.05.target-providers-good-test.png " ")
  Make sure *Connection State* remains *good* and *Last Activity Date* field updated to the current date and time. 


### **2.3 Configure Archiver on the Source WebCenter Content Instance**

1. Launch *Oracle WebCenter Content Administration Utility* application installed in [1.2 Setup Archiver on Target WebCenter Content Instance](../01-target-Archiver-setup/01-target-Archiver-setup.md#1.2InstallOracleWebCenterContentAdministrationUtilityapplication) by navigating to *Administration* --> *Desktop Client Apps*  and clicking on *Launch Client* button 
  ![Desktop Client Apps](images/2.2.01.target-archive-setup.DesktopClient_Launch_Client.png "Desktop Client Apps")
   or by launching *Oracle WebCenter Content Administration Utility* application from your desktop
  ![Desktop Client Apps](images/2.2.01.target-archive-setup.DesktopClient_Launch_Client_from_Desktop.png "Desktop Client Apps")
2. Specify WebCenter Content Administrator Cloud account login credentials and Source WebCenter Content Server URL (for example [https://source-wcc.[domain name].com/cs](https://target-wcc.[domain name].com/cs))
![Desktop Client Apps](images/2.3.2.target-archive-setup.DesktopClient_Connect.png =50%x* "Desktop Client Apps")
Click "OK" button
3. In *WebCenter Administration* app, click on *Archiver*
![Desktop Client Apps](images/03.03.target-archive-setup.WC_Admin_Archiver.png =25%x* "Desktop Client Apps")
Wait for Archiver to load
![Desktop Client Apps](images/03.04.target-archive-setup.Archiver_for_wcgolden1412_4444.png =50%x* "Desktop Client Apps")
4. Click on *Edit* and then *Add* from the Archiver top menu
![Desktop Client Apps](images/03.04.target-archive-setup.Archiver_for_wcgolden1412_4444_ADD.png =50%x* "Desktop Client Apps")

5. Populate Archive Name and Description and click *OK* button
![Desktop Client Apps](images/03.05.source-archive-setup.Archiver_created.png =50%x* "Desktop Client Apps")

### **2.4 Add Target Collection to Source Archiver**

1. Select newly created "SourceArchiver" and click on *Options* --> *Open Archive Collections* option.
![](images/04.01.png =50%x* "")

2. Click on *Browse Proxied * button.
![](images/04.02.png =50%x* "")

3. In *Proxied Servers* dialog, select Source Instance name and then select Associated Source Collection Name. 
![](images/04.03.png =50%x* "")
Click on *OK* button.

4. Make sure selected Source collection is now displayed in the list of Collections
![](images/04.04.png =50%x* "")
Close *Collections* dialog. 




### **2.5 Configure *Transfer Destination* in Source Archiver to Target Archiver**

1. Click on *Transfer To* and *Edit* button of *Transfer Destinageion* section
![](images/05.01.png =50%x* "")
2. Select Target Collection and Target Archive
![](images/05.02.png =50%x* "")
Click *OK" botton
3. Make sure *Transfer To* has *Transfer Owner* and *Target Archive* populated
![](images/05.03.png =50%x* "")



You may now **proceed to the next lab**.

## Acknowledgements

* **Authors-** Nazar Doroshenko, Development Manager, Oracle WebCenter Content
* **Contributors-** Sameer Chikkerur, Mandar Tengse
* **Last Updated By/Date-** Nazar Doroshenko, May 2025