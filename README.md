# pcf-azure-install

## Pre-requsities 
1. Bash 
2. Azure CLI
2. Git
3. Github account

[NOTE]
If you are running windows desktop, install virtualBox and Vagrant and create a Lucid64 box 


## Steps to setup Azure Env
1. Using a browser log into your Azure portal
2. Create a new `resource group` and make note of the name. 
3. `git clone https://github.com/yjayaraman-pivotal/pcf-azure-install.git ` or download https://github.com/yjayaraman-pivotal/pcf-azure-install/archive/master.zip
3. From a terminal window, run setup_azure_env.sh
4. Once the env is setup, using a Browser log into your Azure portal
5. Create a jumpbox (coming soon in the script)
6. SSH into the jumpbox
7. sudo apt-get update && sudo apt-get install git
8. `git clone https://github.com/yjayaraman-pivotal/pcf-azure-install.git ` or download https://github.com/yjayaraman-pivotal/pcf-azure-install/archive/master.zip
9. cd to the <checkout directory>/scripts
10. Run setupbosh.sh
11. Copy <checkout directory>//templates/bosh.cnf ~/manifests/deployments/bosh.yml
12. cd manifests/deployments
13. ssh-keygen -t rsa -f ~/bosh -P "" -C ""
13. modify bosh.yml (to update it with your Azure info, put the ssh info, etc.), Look for variables starting __ and replace it with the appropriate values


To be continued ....



