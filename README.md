# Azure-VM-Deployment

## Creating a Linux VM in Azure

Step 1: Type "virtual machines" into the search function in your Azure Portal.

Step 2: Click "Create" and then "Virtual Machine"

Step 3: Select a Resouce group from the dropdown or click "create new" and enter a name for your resource group.

Step 4: Name your virtual machine, select a region and select an image (OS)

Step 5: Select the size of your VM, which includes number of VCPU and RAM.

Step 6: Click the "review and create" button at the bottom of the page, double check the configuration and then select "create".

Step 7: Download the private key and make sure to save it.

## Connecting to a Virtual Machine

### To conenct to the VM using SSH from a Windows device follow the steps below

Step 1: Open Powershell and run the following command:ssh -i "Pem file path" azureuser@"VM IPv4 address"

Step 2: Change "Pem file path" to rhe file path where you saved the Private key.

Step 3: Change the "VM IPV4 address" to the Public IP address of the VPN.

Step 4: If done correctly you sohlud be connected to VM via SSH.

## Installing a web server

Run the following commands while connected to the VM: 
sudo apt-get -y update
sudo apt-get -y install nginx

Once complete type the virtual machine's public IP address into a web browser to verify nginx is installed.


