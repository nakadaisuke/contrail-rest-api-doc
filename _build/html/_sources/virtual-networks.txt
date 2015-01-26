====================
virtual-networks
====================

 Virtual networks include Virtual-network,Subnet,Routing instance, Route target, VXLAN Network Identifier and so on.

virtual-networks Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " virtual-network " string " No " CR " generated " N/A " The display name
   fq_name " virtual-network " list(str) " Yes " CR " [] " Valid form <domain>,<project>,<name> " The full query name of this attribute
   id_perms " virtual-network " N/A " No " CRU " N/A " N/A " The root of this attribute
   created " id_perms " datetime " No " R " generated " N/A " The date time of created date of this attribute
   description " id_perms " string " No " CRU " null " N/A " The description of this attribute
   enable " id_perms " bool " No " CRU " true " Valid form {true|false} " Specifies whethere this attribute is enable or not
   last_modified " id_perms " datetime " No " R " generated " N/A " The date time of modified date of this attribute
   permissions " id_perms " list(dict) " No " CRU " generated " N/A " The owner and access level
   group " permissions " string " No " CRU " generated " N/A " The group of this attribute
   group_access " permissions " int " No " CRU " generated " 0-7 " The access type of group
   other_access " permissions " int " No " CRU " generated " 0-7 " The access type of others
   owner " permissions " string " No " CRU " generated " N/A " The name of the ownter of this attribute
   owner_access " permissions " int " No " CRU " generated " 0-7 " The access type of the ownter
   user_visible " id_perms " bool " No " CRU " true " Valid form {true|false} " Specifies whethere this attribute is visible by user or not
   uuid " id_perms " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid " int " No " R " generated " N/A " For internal use
   uuid_mslong " uuid " int " No " R " generated " N/A " For internal use
   instance_ip_back_refs " virtual-network " N/A " No " CRUD " generated " N/A " The instance IP which belongs to this network
   attr " instance_ip_back_refs " string " No " R " generated " N/A " The attribute of this list
   href " instance_ip_back_refs " string " No " R " generated " N/A " The URI of this attribute
   to " instance_ip_back_refs " list(str) " No " CR " [] " Valid form <uuid> " The list of this attribute
   uuid " instance_ip_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   is_shaerd " virtual-network " bool " No " CRU " false " Valid form {true|false} " Specifies whether the network resource can be accessed by any project or not
   name " virtual-network " string " No " CRU " generated " N/A " The name of thie attribute
   network_ipam_refs " virtual-network " N/A " No " CR " N/A " N/A " The root of this attribute
   attr " network_ipam_refs " N/A " No " CRUD " null " N/A " The root of this attribute
   host_routes " attr " list(route table) " No " CRU " [] " Valid route table type " The host route list
   ipam_subnets " attr " N/A " No " CRD " [] " N/A " The root of this attribute
   addr_from_start " ipam_subnets " bool " No " CRU " true " Valid form {true|false} " Specifies whehter the network allocation start from low value or high value
   allocation_pools " ipam_subnets " list(dict) " No " CRU " [] " N/A " The IP address pool
   end " allocation_pools " string " No " CRUD " null " Valid IP address " The end of IP address of allocation pool
   start " allocation_pools " string " No " CRUD " null " Valid IP address " The start of IP address of allocation pool
   default_gateway " ipam_subnets " string " No " CRUD " first address in cidr " Valid IP address " The dafault gateway
   dhcp_option_list " ipam_subnets " string " No " CRU " null " N/A " For internal use
   dns_nameservers " ipam_subnets " list(str) " No " CRU " [] " Valid IP address " The list of DNS servers
   dns_server_address " ipam_subnets " string " No " CRUD " generated " Valid IP address " The DNS proxy IP address
   enable_dhcp " ipam_subnets " bool " No " CRU " true " Valid form {true|false} " Specifies whether DHCP is enable or not
   host_routes " ipam_subnets " list(str) " No " CRUD " null " Valit list of IP address " The list of route which is published by DHCP server
   subnet " ipam_subnets " N/A " No " CRD " N/A " N/A " The root of this attribute
   ip_prefix " subnet " string " No " CRD " null " Valid network address " The network address of the subnet
   ip_prefix_len " subnet " int " No " CRD " null " Valid IP prefix " The prefix of the subnet
   subnet_name " ipam_subnets " string " No " CRUD " null " N/A " The name of subnet
   subnet_uuid " ipam_subnets " uuid-str " No " CR " generated " N/A " The UUID of this attribute
   href " network_ipam_refs " string " No " R " generated " N/A " The URI of this attribute
   to " network_ipam_refs " list(str) " Yes " CR " [] " Valid IPAM form <domain>,<project>,<IPAM> " The list of this attribute
   uuid " network_ipam_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   parent_href " virtual-network " string " No " R " generated " N/A " The URI of this attribute
   parent_type " virtual-network " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " virtual-network " uuid-str " No " R " generated " N/A " The UUID of this attribute
   router_external " virtual-network " bool " No " CRU " false " Valid form  {true|false} " Specifies whether the network resouse can be allocated on External network
   routing_instances " virtual-network " string " No " CR " N/A " N/A " The root of this attribute
   href " routing_instances " string " No " R " generated " N/A " The URI of this attribute
   to " routing_instances " list(str) " No " R " generated " N/A " The list of this attribute
   uuid " routing_instances " uuid-str " No " R " generated " N/A " The uuid of routing instance
   uuid " virtual-network " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_machine_interface_back_refs " virtual-network " string " N/A " R " generated " N/A " The root of this attribute
   attr " virtual_machine_interface_back_refs " string " No " R " generated " N/A " The list of this attribute
   href " virtual_machine_interface_back_refs " string " No " R " generated " N/A " The URI of the interface
   to " virtual_machine_interface_back_refs " list(str) " No " R " generated " N/A " The list of this attribute
   uuid " virtual_machine_interface_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_network_properties " virtual-network " string " N/A " CRU " N/A " N/A " The root of this attribute
   allow_transit " virtual_network_properties " bool " No " CRU " null " N/A " Virtula network is either Transit or not
   forwarding_mode " virtual_network_properties " string " No " CRU " null " Valid form {l2_l3|l2} " Forwarding mode for virtual-network
   network_id " virtual_network_properties " int " No " R " generated " N/A " A unique id for the network, auto generated
   vxlan_network_identifier " virtual_network_properties " integer " No " CRU " null " Valid VNI range " VNI for the network

virtual-networks JSON
====
.. highlight:: json
   :linenothreshold: 5

::

  {
      "virtual-network": {
          "display_name": "<NAME>",
          "fq_name": [
              "<DOMAIN>",
              "<PROJECT>",
              "<NAME>"
          ],
          "href": "http://<API-SERVER>/virtual-network/<UUID>",
          "id_perms": {
              "created": "<DATE>",
              "description": null,
              "enable": true,
              "last_modified": "<DATE>",
              "permissions": {
                  "group": "<GROUP>",
                  "group_access": 7,
                  "other_access": 7,
                  "owner": "<OWNER>",
                  "owner_access": 7
              },
              "user_visible": true,
              "uuid": {
                  "uuid_lslong": <INTEGER>,
                  "uuid_mslong": <INTEGER>
              }
          },
          "instance_ip_back_refs": [
              {
                  "attr": null,
                  "href": "http://<API-SERVER>/instance-ip/<UUID>",
                  "to": [
                      "<UUID>"
                  ],
                  "uuid": "<UUID>"
              }
          ],
          "is_shared": false,
          "name": "<NAME>",
          "network_ipam_refs": [
              {
                  "attr": {
                      "host_routes": null,
                      "ipam_subnets": [
                          {
                              "addr_from_start": true,
                              "allocation_pools": [
                                  {
                                      "end": "<IP_ADDRESS>",
                                      "start": "<IP_ADDRESS>"
                                  }
                              ],
                              "default_gateway": "<IP_ADDRESS>",
                              "dhcp_option_list": null,
                              "dns_nameservers": [],
                              "dns_server_address": "<IP_ADDRESS>",
                              "enable_dhcp": true,
                              "host_routes": null,
                              "subnet": {
                                  "ip_prefix": "<IP_ADDRESS>",
                                  "ip_prefix_len": <PREFIX>
                              },
                              "subnet_name": "",
                              "subnet_uuid": "<UUID>"
                          }
                      ]
                  },
                  "href": "http://<API-SERVER>/network-ipam/<UUID>",
                  "to": [
                      "<DOMAIN>",
                      "<PROJECT>",
                      "<IPAM>"
                  ],
                  "uuid": "<UUID>"
              }
          ],
          "parent_href": "http://<API-SERVER>/project/<UUID>",
          "parent_type": "project",
          "parent_uuid": "<UUID>",
          "router_external": false,
          "routing_instances": [
              {
                  "href": "http://<API-SERVER>/routing-instance/<UUID>",
                  "to": [
                      "<DOMAIN>",
                      "<PROJECT>",
                      "<NAME>",
                      "<NAME>"
                  ],
                  "uuid": "<UUID>"
              }
          ],
          "uuid": "<UUID>",
          "virtual_machine_interface_back_refs": [
              {
                  "attr": null,
                  "href": "http://<API-SERVER>/virtual-machine-interface/<UUID>",
                  "to": [
                      "<DOMAIN>",
                      "<PROJECT>",
                      "<UUID>"
                  ],
                  "uuid": "<UUID>"
              }
          ],
          "virtual_network_properties": {
              "allow_transit": null,
              "forwarding_mode": null,
              "network_id": <INTEGER>,
              "vxlan_network_identifier": null
          }
      }
  }
