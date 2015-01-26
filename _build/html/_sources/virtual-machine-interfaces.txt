====================
virtual-machine-interface
====================

 virtual-machine-interface includes instance IP,routing instance,service chain and so on

virtual-machine-interfaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " virtual-machine-interface " string " No " CR " generated " N/A " The display name
   floating_ip_back_refs " virtual-machine-interface " list(str) " No " R " generated " N/A " The root of this attribute
   attr " floating_ip_back_refs " N/A " No " R " generated " N/A " The root of this attribute
   href " floating_ip_back_refs " string " No " R " null " Valid MAC address " The destination MAC address
   to " floating_ip_back_refs " list(str) " No " R " [] " Valid IPAM form <domain>,<project>,<network>,<attribute>,<name> " The list of this attribute
   uuid " floating_ip_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   fq_name " virtual-machine-interface " list(str) " Yes " CR " [] " Valid form <domain>,<project>,<name> " The full query name of this attribute
   href " virtual-machine-interface " string " No " R " null " Valid MAC address " The destination MAC address
   id_perms " virtual-machine-interface " N/A " No " CRU " N/A " N/A " The root of this attribute
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
   instance_ip_back_refs " virtual-machine-interface " list(str) " No " R " generated " N/A " The root of this attribute
   attr " instance_ip_back_refs " N/A " No " R " generated " N/A " The root of this attribute
   href " instance_ip_back_refs " string " No " R " null " Valid MAC address " The destination MAC address
   to " instance_ip_back_refs " list(str) " No " R " [] " Valid IPAM form <name> " The list of this attribute
   uuid " instance_ip_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   name " virtual-machine-interface " string " No " CRU " generated " N/A " The name of thie attribute
   parent_href " virtual-DNS " string " No " R " generated " N/A " The URI of this attribute
   parent_type " virtual-DNS " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " virtual-DNS " uuid-str " No " R " generated " N/A " The UUID of this attribute
   routing_instance_refs " virtual-machine-interface " list(str) " No " CR " N/A " N/A " The root of this attribute
   attr " routing_instance_refs " N/A " No " CRU " null " N/A " The root of this attribute
   direction " attr " string " No " R " generated " Valid form {ingress|egress|both} " The direction type
   dst_mac " attr " string " No " R " null " Valid MAC address " The destination MAC address
   mpls_label " attr " integer " No " R " Null " N/A " The MPLS label value
   protocol " attr " string " No " R " Null " Valid form {tcp|udp|icmp|any} " The protocol type
   service_chain_address " attr " string " No " R " Null " Valid IP address " The service chain address
   src_mac " attr " string " No " R " null " Valid MAC address " The source MAC address
   vlan_tag " attr " integer " No " R " null " Valid MAC address " The VLAN ID
   direction " attr " string " No " R " generated " Valid form {ingress|egress|both} " The direction type
   dst_mac " attr " string " No " R " null " Valid MAC address " The destination MAC address
   mpls_label " attr " integer " No " R " Null " N/A " The MPLS label value
   protocol " attr " string " No " R " Null " Valid form {tcp|udp|icmp|any} " The protocol type
   service_chain_address " attr " string " No " R " Null " Valid IP address " The service chain address
   src_mac " attr " string " No " R " null " Valid MAC address " The source MAC address
   vlan_tag " attr " integer " No " R " null " Valid MAC address " The VLAN ID
   href " routing_instance_refs " string " No " R " null " Valid MAC address " The destination MAC address
   to " routing_instance_refs " list(str) " Yes " R " [] " Valid IPAM form <domain>,<project>,<network>,<name> " The list of this attribute
   uuid " routing_instance_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   security_group_refs " virtual-machine-interface " list(str) " No " CR " N/A " N/A " The root of this attribute
   to " security_group_refs " list(str) " Yes " CRU " [] " Valid form <domain>,<project>,<name> " The list of this attribute
   href " security_group_refs " string " No " R " null " Valid MAC address " The destination MAC address
   attr " security_group_refs " N/A " No " CRU " null " N/A " The root of this attribute
   uuid " security_group_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid " virtual-machine-interface " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_machine_interface_device_owner " virtual-machine-interface " string " Yes " CR " N/A " Valid AZ " The virtual machine interface AZ
   virtual_machine_interface_mac_addresses " virtual-machine-interface " N/A " No " CR " N/A " N/A " The root of this attribute
   mac_address " virtual_machine_interface_mac_addresses " list(str) " No " CRUD " [] " Valid MAC address " The MAC address list
   virtual_machine_interface_properties " virtual-machine-interface " N/A " No " CR " N/A " N/A " The root of this attribute
   interface_mirror " virtual_machine_interface_properties " string " No " CRUD " null " N/A " The interface mirror destination
   local_preference " virtual_machine_interface_properties " integer " No " CRUD " null " N/A " The local preference
   service_interface_type " virtual_machine_interface_properties " string " No " CRUD " null " Valid form {management|left|right|other} " The service interface type
   sub-interface-vlan-tag " virtual_machine_interface_properties " integer " No " CRUD " null " N/A " The vlan tag of sub interface
   virtual_machine_refs " virtual-machine-interface " list(str) " No " CR " N/A " N/A " The root of this attribute
   attr " virtual_machine_refs " N/A " No " CRU " null " N/A " The root of this attribute
   href " virtual_machine_refs " string " No " R " null " Valid MAC address " The destination MAC address
   to " virtual_machine_refs " list(str) " Yes " CRU " [] " Valid form <domain>,<project>,<name> " The list of this attribute
   uuid " virtual_machine_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_network_refs " virtual-machine-interface " list(str) " No " CR " N/A " N/A " The root of this attribute
   attr " virtual_network_refs " N/A " No " CRU " null " N/A " The root of this attribute
   href " virtual_network_refs " string " No " R " null " Valid MAC address " The destination MAC address
   to " virtual_network_refs " list(str) " Yes " CRU " [] " Valid form <domain>,<project>,<name> " The list of this attribute
   uuid " virtual_network_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute

virtual-machine-interfaces JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-machine-interface": {
           "display_name": "1ae35391-f7c3-4b80-9fdc-9963e6568c02",
           "floating_ip_back_refs": [
               {
                   "attr": null,
                   "href": "http://127.0.0.1:8082/floating-ip/57cc5f42-fd35-45c0-a372-ef7d014e5377",
                   "to": [
                       "default-domain",
                       "admin",
                       "customer_public",
                       "default",
                       "57cc5f42-fd35-45c0-a372-ef7d014e5377"
                   ],
                   "uuid": "57cc5f42-fd35-45c0-a372-ef7d014e5377"
               }
           ],
           "fq_name": [
               "default-domain",
               "admin",
               "1ae35391-f7c3-4b80-9fdc-9963e6568c02"
           ],
           "href": "http://127.0.0.1:8082/virtual-machine-interface/1ae35391-f7c3-4b80-9fdc-9963e6568c02",
           "id_perms": {
               "created": "2015-01-21T12:16:39.055823",
               "description": null,
               "enable": true,
               "last_modified": "2015-01-21T12:16:39.446600",
               "permissions": {
                   "group": "admin",
                   "group_access": 7,
                   "other_access": 7,
                   "owner": "admin",
                   "owner_access": 7
               },
               "user_visible": true,
               "uuid": {
                   "uuid_lslong": 11519250601252129794,
                   "uuid_mslong": 1937484151091579776
               }
           },
           "instance_ip_back_refs": [
               {
                   "attr": null,
                   "href": "http://127.0.0.1:8082/instance-ip/9af429a0-f5e2-40eb-ba30-98f6ecaf86e2",
                   "to": [
                       "9af429a0-f5e2-40eb-ba30-98f6ecaf86e2"
                   ],
                   "uuid": "9af429a0-f5e2-40eb-ba30-98f6ecaf86e2"
               }
           ],
           "name": "1ae35391-f7c3-4b80-9fdc-9963e6568c02",
           "parent_href": "http://127.0.0.1:8082/project/9e5ba4c4-33f8-422c-8300-06a02e8ebab6",
           "parent_type": "project",
           "parent_uuid": "9e5ba4c4-33f8-422c-8300-06a02e8ebab6",
           "routing_instance_refs": [
               {
                   "attr": {
                       "direction": "both",
                       "dst_mac": null,
                       "mpls_label": null,
                       "protocol": null,
                       "service_chain_address": null,
                       "src_mac": null,
                       "vlan_tag": null
                   },
                   "href": "http://127.0.0.1:8082/routing-instance/5ab05ed4-7f71-4299-9015-6ab7cda4bd37",
                   "to": [
                       "default-domain",
                       "admin",
                       "mac1",
                       "mac1"
                   ],
                   "uuid": "5ab05ed4-7f71-4299-9015-6ab7cda4bd37"
               }
           ],
           "security_group_refs": [
               {
                   "attr": null,
                   "href": "http://127.0.0.1:8082/security-group/381b8ea3-0b33-4ee0-8d13-6d2ee76ac540",
                   "to": [
                       "default-domain",
                       "admin",
                       "default"
                   ],
                   "uuid": "381b8ea3-0b33-4ee0-8d13-6d2ee76ac540"
               }
           ],
           "uuid": "1ae35391-f7c3-4b80-9fdc-9963e6568c02",
           "virtual_machine_interface_device_owner": "compute:nova",
           "virtual_machine_interface_mac_addresses": {
               "mac_address": [
                   "02:1a:e3:53:91:f7"
               ]
           },
           "virtual_machine_interface_properties": {
               "interface_mirror": null,
               "local_preference": null,
               "service_interface_type": "left"
           },
           "virtual_machine_refs": [
               {
                   "attr": null,
                   "href": "http://127.0.0.1:8082/virtual-machine/7a39517d-8f1c-4c3c-9b89-5fd055f20350",
                   "to": [
                       "7a39517d-8f1c-4c3c-9b89-5fd055f20350"
                   ],
                   "uuid": "7a39517d-8f1c-4c3c-9b89-5fd055f20350"
               }
           ],
           "virtual_network_refs": [
               {
                   "attr": null,
                   "href": "http://127.0.0.1:8082/virtual-network/a8d51c18-b4f8-4309-a28f-d185a39c86c2",
                   "to": [
                       "default-domain",
                       "admin",
                       "mac1"
                   ],
                   "uuid": "a8d51c18-b4f8-4309-a28f-d185a39c86c2"
               }
           ]
       }
   }
