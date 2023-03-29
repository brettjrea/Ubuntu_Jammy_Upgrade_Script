#### Title: "Node.js and Build Tools Installation Guide with Optional OS Upgrades"

  <details>
  <summary>1. Get Debian/Ubuntu:</summary>
  1. [Install WSL Debian on Windows](https://github.com/brettjrea/Windows_WSL_Debian)
  2. [Install WSL Ubuntu on Windows](https://github.com/brettjrea/Windows_WSL_Ubuntu)
  3. [Install VSCode with Remote Pack on Windows](https://github.com/brettjrea/Windows_VSC_Remote_Pack)
  </details>

  <details>
  <summary>2. Optional OS upgrades:</summary>  
  1. [Upgrade Debian Bullseye to Buster](https://github.com/brettjrea/Debian_Bullseye_Upgrade_Script)
  2. [Upgrade Ubuntu Focal to Jammy](https://github.com/brettjrea/Ubuntu_Jammy_Upgrade_Script)
  </details>
  
  <details>
  <summary>3. Node.js tools:</summary>  
  1. [Install NVM](https://github.com/brettjrea/Debian_Install_NVM) - Node Version Manager
  2. [Install NVS](https://github.com/brettjrea/Debian_Install_NVS) - Node Version Switcher (added 02/23 it is a cross-platform node based successor/replacement for NVM)
  </details>
  
  <details>     
  <summary>4. Build tools:</summary>       
  1. [Install common build tools.](https://github.com/brettjrea/Debian_Install_Common_Build_Tools)
  </details>
  
  <details>   
  <summary>5. Add a Backend:</summary> 
  1. [Install Strapi.io backend](https://github.com/brettjrea/Debian_Strapi_Backend_API)
  </details>
  
  <details>   
  <summary>7. Add a Frontend:</summary> 
  1. [Install Gatsby frontend](https://github.com/brettjrea/Debian_Gatsby_Frontend_Client)
  </details>
  
  <details>   
  <summary>8. Configure Process Manager:</summary> 
  1. [Configure PM2 Process Manager](https://github.com/brettjrea/Debian_Configure_PM2)
  </details>
  
  <details>   
  <summary>9. Add GitHub CLI:</summary> 
  1. [Install GitHub CLI](https://github.com/brettjrea/Debian_Install_GitHub_CLI)
  </details>
---
### Upgrade Ubuntu Focal to Jammy with upgrade.sh

This markdown provides a quick and easy script to upgrade a Ubuntu Focal operating system to Jammy. The script has been verified as still working in 2022, although it may require the manual installation of wget.

To upgrade Ubuntu Focal to Jammy with upgrade.sh run the following commands:

```
sudo apt upgrade -y && sudo apt update -y && sudo apt autoremove -y &&
sudo apt install wget -y &&
sudo apt-get install --reinstall ca-certificates -y &&
wget https://raw.githubusercontent.com/brettjrea/Scripts_Fix/master/fixscripts.sh &&
wget https://raw.githubusercontent.com/brettjrea/Ubuntu_Jammy_Upgrade_Script/master/upgrade.sh &&
sudo bash fixscripts.sh &&
sudo bash upgrade.sh && 
sudo apt autoremove -y &&
sudo apt clean -y
set -o emacs
```
