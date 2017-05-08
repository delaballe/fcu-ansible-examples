This project is a tweak of the Ansible ec2 modules to nativelly and easly manage cloud architectures on the [Outscale® Cloud Platform](https://www.outscale.com) using [Ansible](https://github.com/ansible/ansible).

As it is based on an  Ansible 2.2.1 It allow you to use all the features natively supported by Ansible, it is by default bundled with :

 - [ansible](https://github.com/ansible/ansible)
 - [ansible-playbook](http://docs.ansible.com/ansible/playbooks.html)
 - [ansible-galaxy](https://github.com/ansible/galaxy)
 - [ansible-vault](http://docs.ansible.com/ansible/playbooks_vault.html)
 - [ansible-lint](https://github.com/willthames/ansible-lint)

fcu-ansible expose an fcu namespace that you can use in your playbooks exactly the same way you do with the native Ansible ec2 modules.

Every ec2_XXXX ansible module have it's fcu equivalent fcu_XXXX.

This allow you to use both fcu and ec2 in the same playbook which offer you the possibility to deploy cross cloud operators architectures in one playbook.

Bellow is the list of the Cloud Objects that you can Provision and manage in their entire lifecycle (Create / Update / Delete) with fcu-ansible :

- [VPCs](https://wiki.outscale.net/display/DOCU/About+Virtual+Private+Clouds)
- [Subnets](https://wiki.outscale.net/display/DOCU/Creating+a+Subnet+in+a+VPC)
- [Route Tables](https://wiki.outscale.net/display/DOCU/About+Route+Tables)
- Internet gateways
- NAT Gateways
- Keypairs (dynamically generated or not)
- VPC Peering Connections
- VPN Connections
- External IPs
- Security Groups
- Virtual Private Gateways
- Fexible Compute Units Instances
- Volumes
- Snapshots
- Outscale Marchine Images
- Instances

Once your cloud Architectures are provisioned and your Compute Units are up, in one shot, you can orchestrate complex and heterogenous application deployment with all the flexibility and killer features that Ansible offer.

It also include [fcu-ansible-inventory](https://github.com/delaballe/fcu-ansible-inventory) which is a [state of the art Ansible Dynamic Inventory](https://docs.ansible.com/ansible/dev_guide/developing_inventory.html), specially built to work in the [Outscale Cloud Platform](https://www.outscale.com).

## Dependencies

- python >= 2.7  
- virtualenv  
- pip  
- fcu-boto  
- fcu-ansible-lib   
