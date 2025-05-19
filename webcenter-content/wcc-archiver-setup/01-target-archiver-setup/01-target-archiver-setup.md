# Prepare Setup

## Introduction

This lab will show you how to setup the Archiver, a Java applet, on the Target WebCenter Content Instance.


**Estimated Lab Time**: *TBD*

### Objectives

- Setup the Archiver on Target WebCenter Content Instance
- Prepare Target Content Instance required parameters for the Archiver Configuration on the Source Content Instance.


## Task 1: Setup Archiver on Target WebCenter Content Instance
### **1.1 Sign in to WebCenter Content Administration UI**

  1. Go to the Target WebCenter Content. For example `https://target-wcc.mydomain.com/cs` 
  ![Administration UI Login](images/target-archive-setup.01.AdminLogin.png "Administration UI Login")

  2. Enter your WebCenter Content Administrator Cloud account login credentials
  ![OCI Login](images/target-archive-setup.02.TenancyLogin.png "OCI Login")

  3. Click on "Sign In" button 
  ![Administration UI](images/target-archive-setup.03.WebCenter_Admin_UI.png "Administration UI")



### **1.2 Install Oracle WebCenter Content Administration Utility application**

1. Navigate to *Administration* --> *Desktop Client Apps*  and click *Download Client* button to download *wccadmin-installer.dmg* installer for MacOS or *wccadmin-installer.exe* installer for MS Windows
  ![Desktop Client Apps](images/02.01.target-archive-setup.DesktopClient.png "Desktop Client Apps")

2. Once *wccadmin-installer.dmg* downloaded, double-click on the installer to install the *Oracle WebCenter Content Administration* Utility application 
  ![](images/02.02.target-archive-setup.Install_WC_Administration_Utility.png =35%x*)

3. Follow onscreen instructions to complete the installation



### **1.3 Configure Archiver on the Target WebCenter Content Instance**

1. Launch WebCenter Administration utility by navigating to *Administration* --> *Desktop Client Apps*  and clicking on *Launch Client* button 
  ![Desktop Client Apps](images/03.01.target-archive-setup.DesktopClient_Launch_Client.png "Desktop Client Apps")
 or launching *Oracle WebCenter Content Administration Utility* application from your desktop
  ![Desktop Client Apps](images/2.2.01.target-archive-setup.DesktopClient_Launch_Client_from_Desktop.png "Desktop Client Apps")

2. Specify WebCenter Content Administrator Cloud account login credentials and Target WebCenter Content Server URL (for example `https://target-wcc.mydomain.com/cs` )
![Desktop Client Apps](images/03.02.target-archive-setup.DesktopClient_Connect.png =50%x* "Desktop Client Apps")
Click "OK" button
3. In *WebCenter Administration* app, click on *Archiver*
![Desktop Client Apps](images/03.03.target-archive-setup.WC_Admin_Archiver.png =25%x* "Desktop Client Apps")
Wait for Archiver to load
![Desktop Client Apps](images/03.04.target-archive-setup.Archiver_for_targetwcc_4444.png =50%x* "Desktop Client Apps")
4. Click on *Edit* and then *Add* from the Archiver top menu
![Desktop Client Apps](images/03.04.target-archive-setup.Archiver_for_targetwcc_4444_ADD.png =50%x* "Desktop Client Apps")

5. Populate Archive Name and Description and click *OK* button
![Desktop Client Apps](images/03.05.target-archive-setup.Archiver_for_targetwcc_4444_ADD.png =50%x* "Desktop Client Apps")

6. Select newly created "TargetArchiver" and click on *Transfer To* tab. Click on *Edit* button of *Transfer Options* section
![Desktop Client Apps](images/03.06.target-archive-setup.Archiver_for_targetwcc_4444_IsTargetable.png =50%x* "Desktop Client Apps")
Check *Is Targetable* checkbox and click *OK* button

7. Exit from *Archiver* and *WebCenter Administraiton* App
![Desktop Client Apps](images/03.07.target-archive-setup.Archiver.png =50%x* "Desktop Client Apps")
![Desktop Client Apps](images/03.07.target-archive-setup.WC_Administration.png =25%x* "Desktop Client Apps")


### **1.3 Archiver Connection Informaiton for Source Archiver configuration**

1. In Target WebCenter Content Instance, navigate to *Administration* --> *Configuration Information for [System Name]* and then click on *System Configuration*
![Desktop Client Apps](images/04.01.target-archive-setup.TargetServerConfiguration.png "Desktop Client Apps")
Note the values for the following parameters:
- **Instance Name**
- **Server Port**
- **Http Web Root**
- **HTTP Server Address**


 


You may now **proceed to the next lab**.

## Acknowledgements

* **Authors-** Nazar Doroshenko, Development Manager, Oracle WebCenter Content
* **Contributors-** Sameer Chikkerur, Mandar Tengse
* **Last Updated By/Date-** Nazar Doroshenko, May 2025