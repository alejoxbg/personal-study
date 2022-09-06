![[Pasted image 20220827095207.png]]

Vpc Peering is the way we ocnnect to VPC different.

A VPC is assosiated to a proyect so if we have different projects we need to define different VPCs. If every Project is asosiated to a different team, in each team we will need a person with the knowledge of the managment and administration of VPCs.

What happen if we want to centralice the managment of all the comunications, but we want that every project acn access to the same mechanism of network defined.

That is a shared VPC. We define a network with all the resources defined as firewall rules, different sub networks, IP ranges, etc. This project is called Host, and is usefull to give to other projects the service that they ask for. So you will have a central project of contraliced and managment of comunnications administrated by a single team and there are different projects that only will use the network resources that define this team of networking.

whit this you can centraliced, simplify and be more secure.

![[Pasted image 20220827095845.png]]



Firewall rules allows you to determine what services can comunnicate with others or which services can't comunnicate with others, increasing with that the security capabilities. 

There are igress rules, ingress rules are tags added to the servis that ask for something, this service has the tag and the VPC read the tag to give the configurated acces to them. Another way to identificate the services is because it has a IP asignated and we allow this IP in the firewall rule.

The target is the team that will paly this firewall rule, and this group allow or deny the comunication between them.

so there are 2 different rules the ingress and the egress, the ingress is when something is trying to sent something, so the data ingress the VPC and we can have an ingress firewall rule that allows or deny the comunnication based in a ingress rule (TAG or service accoun) so the origin server has the permits to sent information. in the other side there is a egress firewall, when the origin server send the data to the VPC it check also the egress permits, the egress permit is also configured to the destiny service, and the egress rule with a tac ot a service account can allow or deny the entry of data.

![[Pasted image 20220827100843.png]]


There are some implicit firewall rules that GCP create, the first one is that all the traffic that goes to internet is allowed, so every VM can connect to internet it can do it. The another one is that the entry traffic to the VM is bloqued and all the communications is restricted.

You can change this behivor with explicit rules.








