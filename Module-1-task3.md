# Create Test VMs and connect to Segment

## Create Test VMs
Now that we have our networks created, we can deploy virtual machines and ensure we can get an IP address from DHCP. Go ahead and Login into your AVS vCenter.

# Exercise 1: Create a Content Library

1. Search **Azure VMware Solution (1)** and then select **Azure VMware Solution (2)**.

   ![](./Images/3.1.png "Select Azure VMware Solution")

1. Select your **Azure VMware Solution**.
1. On the Azure VMware Solution page click on **VMware credentials (1)** under Manage tab and then copy the **Web client URL**, **Username** and **Password** under vCenter Server Credentials **(2)** and paste it in notepad for later use.

   ![](./Images/3.2.jpg)

1. Open a new tab in the Microsoft Edge browser, Enter the **Web Client URL** that you copied in step 3. 

   ![](./Images/new3..2.jpg)

1. Log in to the **VMware vSphere**; Enter the **Username** and **password** that you copied in step 3 and click on **LOGIN**.

   ![](./Images/3.3.jpg)

1. From AVS vCenter, click on the **Menu (1)** bar and then click on **Content Libraries (2)** under Inventory.

   ![](./Images/3.4.jpg)

1. click on the **CREATE** button to create the **New Content Libraries**.

   ![](./Images/new3.5.png)

1. On the **Name and location** pane; Enter name your Library as **Local-Lib (1)** and click on **NEXT (2)**.

   ![](./Images/3.5.jpg)

1. On the **Configure content library** pane; Leave it as default and click on **NEXT**.

   ![](./Images/3.6.jpg)

1. On the **Apply security policy** pane; Leave it as default and click on **NEXT**.

   ![](./Images/3.7.jpg)

1. On the **Add storage** pane; Select **Storage (1)** and click on **NEXT (2)**.

   ![](./Images/3.8.jpg)

1. On the **Ready to complete** pane; Review your content library settings and click on **FINISH**.

   ![](./Images/3.9.jpg)
   
# Exercise 2: Import Item to Content Library 

1. Click on your newly created Library i.e. **Local-Lib**.

   ![](./Images/3.10.jpg)

1. On the Local-Lib Library, click on **ACTIONS (1)** and then click on **Import item (2)**.

   ![](./Images/3..11.jpg)

1. Under the Source tab, Enter the URL as **https://gpsusstorage.blob.core.windows.net/ovas-isos/workshop-vm.ova (1)** and click on **IMPORT (2)**.

   ![](./Images/3.12.jpg)

1. After Successfully Importing the Source file, click on **Actions** on the top right and click on **Continue**.

   ![](./Images/3.13.jpg)

1. Click on **OVF & OVA Templates (1)**. Under **OVF & OVA Templates (2)**, You will see the **workshop-vm (3)**

   ![](./Images/3.14.jpg)
   
# Exercise 3: Create VMs

1. Select the workshop-vm, right click on **workshop-vm (1)**, and then click on **New VM from This Template... (2)**.

   ![](./Images/3.15.jpg)

1. On the **Select a name and folder** pane; Enter the Virtual machine name as **TestVM (1)** and then Select a location for the virtual machine i.e. **SDDC-Datacenter (2)**, and click on **NEXT (3)**.

   ![](./Images/3.16.jpg)

1. On the **Select a compute resource** pane; Select the destination compute resource for this operation i.e. **Cluster-1 (1)** and click on **NEXT (3)**.

   ![](./Images/3.17.jpg)

1. On the **Review details** pane; you can verify the template details and click on **NEXT**.

   ![](./Images/3.18.jpg)

1. On the **License agreements** pane; Accept the terms and click on **NEXT**.

   ![](./Images/3.19.jpg)

1. On the **Select storage** pane; Select **Storage (1)** and click on **NEXT (2)**.

   ![](./Images/3.20.jpg)

1. On the **Select networks** pane; Select the Destination Network as **Web-Segment** and click on **NEXT**.

   ![](./Images/3.21.jpg)

1. On the **Ready to complete** pane; click on **FINISH**.

   ![](./Images/3.22.jpg)
