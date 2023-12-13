Here I will put some finacial data here for analysis

Questions Regarding Jump Server

Hardware Interface
•	Will any device be provided, such as a laptop, for accessing the Azure development environment and doing development work?
•	What permissions will be granted for downloading and installing development required tools?

Network-Related
•	Will the access to SBI GenAI Lab's Azure dev environment be restricted to only being accessible while being connected to SBI Holding Company LAN network? Or will the dev environment be also accessible from requests outside of the SBI Holding Company LAN Network?
o	If access to SBI GenAI Lab's Azure dev environment would only be accessible from within the SBI LAN network,it would be necessary to get internet access control permissions for allowing specific outbound and inbound internet content such as git push to remote repositories (outbound) or allowing pip installs (inbound) for the development device.
o	Also, considering the above, it would be necessary to allow inbound internet access such as copying files (scp) inside the Azure dev environment to       outside of the dev environment and also copying files from outside of the Azure dev environment to inside the Azure dev environment.  
o	Will the development device also be allowed to have internet access similar to the current office PC's internet access?
•	Would it be possible to directly access the Azure dev environment from the development device, for example a laptop?
o	If a jump server is mandatory, can we have it act as a proxy for various tcp protocols between the development device and the Azure dev environment? I.E. HTTPS, connecting via repositories, SSH, etc
	When setting up the VM OS, we will to do inbound downloading, so we also need external internet access control permissions to be allowed for this.

