# MasternodeSetup

wget -q https://github.com/SapphireCoreCoin/MasternodeSetup/blob/master/masternodeinstall.sh

sudo chmod +x masternodeinstall.sh

./masternodeinstall.sh

When prompted to Enter your SapphireCoreCoin Masternode GEN Key.

Paster your Masternode GEN Key and press enter

Wait till Node is fully Synced with blockchain. For check enter below command.

sap-cli getinfo

When Node Fully Synced enter below command for check masternode status.

sap-cli masternode status
