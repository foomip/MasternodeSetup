# MasternodeSetup
Sapphire Core Masternode Guide
Requirements:
SAP Collateral
Ubuntu 16.04 VPS
SAP Local Wallet
First Step: Local Wallet
1. Download the latest version of the sapphire core wallet
https://github.com/SapphireCoreCoin/SAP/releases
2. Create a new receiving address and send the exact collateral to that address
3. Wait 20 confirmations
4. Go to debug console
5. Get your taxid and masternode genkey for step 2 and step 3
a. Taxid
i. Enter the command: masternode outputs
b. Masternode genkey
i. Enter the command: masternode genkey
6. Save these outputs for step 2 and step 3
Second Step: VPS
1. Purchase an Ubuntu 16.04 VPS
2. Enter the below commands to download SAP daemon onto VPS
wget -q https://raw.githubusercontent.com/SapphireCoreCoin/MasternodeSetup/master/masternodeinstall.sh
sudo chmod +x masternodeinstall.sh
./masternodeinstall.sh
3. Enter your masternode genkey from step 1
Third Step: Local Wallet
1. Go to debug console
2. Open masternode.conf file
3. Enter your masternode info
a. Please follow the example provided in the file
b. Use the taxid and masternode genkey from step 1
4. Save and close file
5. Close the wallet
6. Open wallet
7. Go to masternode tab
8. Select the masternode you want to start
9. Click start alias
Fourth Step: VPS
1. Enter below command to make sure that your masternode has started successfully
sap-cli masternode status
2. If started correctly, you will see the below output
