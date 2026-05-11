# EtherChannel-Configuration
In this project, I will configure the Layer 2 EtherChannel between the Access Layer switches and the Distribution Layer switches. I will then configure a Layer 3 EtherChannel between the multilayer switches. I will then configure routes to allow the PCs to reach Server 1> I will also check the load-balancing methods on each switch and configure it 

<img width="693" height="299" alt="Screenshot 2026-05-09 at 9 30 44 PM" src="https://github.com/user-attachments/assets/7d781d8d-e07e-4640-80e9-586a5d74c8d2" />


## Steps Taken

### 1. Configure a Layer 2 EtherChannel between Access Switch 1 (ASW1) and Distribution Switch 1 using the protocol LACP

- I began by combining interfaces g0/1 and g0/2 in golbal config mode using the interface range command. I created an EtherChannel on the interface range by the "channel-protocol" command using the lacp protocol. I made it visible to the network using the channel-group" command and making the mode "active." I added the same comfigurations in g1/0/3 and g1/0/4 in the DWS1 switch. I also created the channel-group mode in the DSW1 switch to be "active" as well, solidifying the EtherChannel connection between ASW1 and DSW1.

- <img width="1103" height="336" alt="Screenshot 2026-05-09 at 9 39 25 PM" src="https://github.com/user-attachments/assets/eafa4e97-bc7e-4a17-be55-0ecccc0d0ff6" />
