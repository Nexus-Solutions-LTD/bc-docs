# Installation Guide for Cosmos
## Dependencies
Cosmos does not have any dependencies. However, it serves as a dependency for most of our applications within the Business Central ecosystem.
## Installation Steps
### Prerequisites
Before installing Cosmos, ensure that you have:
- Microsoft Dynamics 365 Business Central version 23 (BC230) installed.
### Installation Process
To install Cosmos on-premises, follow these steps:
1. **Obtain the Cosmos App**:
   - Obtain the .app file for the Cosmos version that you want to install (e.g. Nexus_Cosmos_2.0.0.0.app).
   - Copy/Download the app file on your destination server.
2. **Access the Business Central Administration Shell**:
   - Navigate to the Business Central Administration Shell.
   - Run the shell as an administrator.
3. **Publish the App**:
   - Run the following command to publish the app:
     ```powershell
     Publish-NAVApp -ServerInstance YourDynamicsNAVServer -Path ".\Nexus_Cosmos_2.0.0.0.app" -SkipVerification
     ```
   - Replace _YourDynamicsNAVServer_ with your server instance name and the path value with the path of your actual .app file.
   - Further information can be found [here](https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-how-publish-and-install-an-extension-v2#to-install-an-extension-by-using-the-client).
4. **Install the App**:
   - Install the app either via the Administrator Shell or by using the client. Both methods are described in the link above.
5. **Verify Installation**:
    - To confirm that Cosmos is installed correctly, navigate to the Extension Management page, and Cosmos should be among the extensions listed.

      ![image](https://github.com/Nexus-Solutions-LTD/bc-docs/assets/50583599/7e5f96cb-f219-48a9-9bcc-668fe6b094b7)

Congratulations! Cosmos is now installed and ready to be utilized as a dependency for other Business Central applications.
