====================
virtual-machine-interface
====================

 Put here  description of attribute 

virtual-machine-interfaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   routing_instance_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   dst_mac " attr" Type "Requ " CRU " Default " Valid " ABCDE
   protocol " attr" Type "Requ " CRU " Default " Valid " ABCDE
   direction " attr" Type "Requ " CRU " Default " Valid " ABCDE
   mpls_label " attr" Type "Requ " CRU " Default " Valid " ABCDE
   vlan_tag " attr" Type "Requ " CRU " Default " Valid " ABCDE
   src_mac " attr" Type "Requ " CRU " Default " Valid " ABCDE
   service_chain_address " attr" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   security_group_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " security_group_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " security_group_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " security_group_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " security_group_refs" Type "Requ " CRU " Default " Valid " ABCDE
   floating_ip_back_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " floating_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " floating_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " floating_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " floating_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   name " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_device_owner " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   fq_name " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_network_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   instance_ip_back_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_mac_addresses " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_properties " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   local_preference " virtual_machine_interface_properties" Type "Requ " CRU " Default " Valid " ABCDE
   interface_mirror " virtual_machine_interface_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_interface_type " virtual_machine_interface_properties" Type "Requ " CRU " Default " Valid " ABCDE
   mac_address " virtual_machine_interface_mac_addresses" Type "Requ " CRU " Default " Valid " ABCDE


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
