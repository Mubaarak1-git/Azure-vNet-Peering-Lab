# Azure vNet Peering Lab
This lab demonstrates how to configure Virtual Network (vNet) Peering in Microsoft Azure to enable secure, low-latency communication between isolated virtual networks. Through step-by-step guidance and visual documentation, you'll learn how to navigate the Azure portal, create bi-directional peering links, and validate connectivity between resources across networks.

## 📌 Objectives
In this lab I created and configured Virtual Network (vNet) Peering in Azure. vNet Peering allows you to connect two virtual networks, enabling low-latency, high-speed communication between them as if they were part of a single network.
#### 1. Explore Azure Portal Navigation for Network Management
    Gain familiarity with the Azure interface and learn how to locate, configure, and manage virtual networks effectively.
#### 2. Establish vNet Peering Between Two Virtual Networks
    Create and configure peering connections to enable secure, low-latency communication between isolated Azure networks.
#### 3. Configure and Name Peering Links for Operational Clarity
    Practice assigning meaningful names and settings to peering links to support resource tracking, troubleshooting, and long-term maintainability.
#### 4. Implement Bi-Directional Peering for Full Connectivity
    Understand and apply two-way peering configurations to ensure seamless communication across both networks.
## 📸 Screenshots


### Step 1: Navigate to Virtual Networks from Azure Resources  
This screenshot shows the Azure portal's "Resources" section, where various infrastructure components are listed. To begin configuring network connectivity, click on **"Virtual networks"** as highlighted in the blue callout. This will take you to the list of available vNets for peering setup.  

![Navisgate to Virtual Network](Screenshots/Click%20Virtual%20Network%20.png)

### Step 2: Locate vNet-App in the Virtual Network List  
This screenshot shows the list of virtual networks under the "Softweb Development" directory. Each entry includes its name, resource group, and location. To begin peering configuration, locate and click on `vNet-App` from the list of networks in the `PuneRG` resource group.  
![Locate vNet-App](screenshots/Opt%20vNet-App.png)


### Step 3: Review vNet-App Overview and Navigate to Peerings  
This screenshot shows the "Overview" tab of the `VNet-App` virtual network. Key details such as address space, location, and connected devices are visible. To begin configuring peering, click the **"Peerings"** option in the left-hand sidebar under the "Settings" section.  

![vNet-App Overview](Screenshots/Click%20Peering%20.png)

### Step 4: Open the Peerings Tab in vNet-App Settings  
This screen shows the "Peerings" section within the `vNet-App` virtual network settings. Azure highlights that peering enables seamless connectivity between two virtual networks. Click the **"+ Add"** button to begin configuring a new peering link.  

![Open Peerings Tab](Screenshots/Click%20Add.png)

### Step 5: Configure Peering from app-prod to vNet-App
Define the reverse peering link from `app-prod` to `vNet-App`, ensuring access permissions are correctly set and naming the link `app-prod-to-app-prod`.

![Remote Peering Configuration](Screenshots/Peering%20Name%20Field.png)

### Step 6: Finalize Remote Peering Link Selection
Select the appropriate peering link name from the dropdown and confirm the remote network configuration for `VNet-Prod`.

![Finalize Remote Peering](Screenshots/Select%20Virual%20Network.png)

### Step 7: Set Remote Peering Details
This view shows the configuration of the remote virtual network `app-prod`, including access permissions and peering link naming. Ensure both networks allow traffic for full connectivity.

![Remote Peering Configuration](Screenshots/Peering%20Link%20Name%20Field.png)



### Step 8: Confirm Peering Status for VNet-App
After configuration, the peering status for `VNet-App` shows "Connected" and "Synchronized" for both local and remote networks—indicating successful bi-directional peering.

![Peering Status Confirmation](Screenshots/Click%20Add%20REVIEW.png)

### Step 9: Verify Peering with app-east Network
This screenshot shows the peering status between `VNet-App` and `app-east`, confirming that the networks are synchronized and connected.

![Additional Peering Verification](Screenshots/Ensuring%20the%20Peering.png)

