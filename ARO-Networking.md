

![ARO Networking architecture](https://github.com/DreamRivulet/ARO/assets/11328236/6aa2ba2d-afd7-4003-9233-ce5d5e425ab4)


By default there will be a public load balancer created, which provides inbound(route, ngress) and outbound connections for the ARO cluste, this means that there will be public SLB create with pip even for the private ARO cluster(for the outbound connection).

To create a private ARO cluster without a public IP, please [set the outbound-type to  *"UserDefineRoutiing"* when creating the cluster](https://learn.microsoft.com/en-us/azure/openshift/howto-create-private-cluster-4x#create-a-private-cluster-without-a-public-ip-address).
