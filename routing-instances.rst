====================
routing-instance
====================

 Put here  description of attribute 

routing-instances Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " routing-instance" string "No " CR " generated " N/A " The display name 
   fq_name " routing-instance" list(str) "Yes " CR " [] " Valid form <domain>,<project>,<network>,<name>" The full query name of this attribute 
   id_perms " routing-instance" N/A "No " CRU "N/A " N/A " The root of this attribute
   created " id_perms" datetime "No " R " generated " N/A " The date time of created date of this attribute 
   description " id_perms" string "No " CRU " null " N/A " The description of this attribute
   enable " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is enable or not 
   last_modified " id_perms" datetime "No " R " generated " N/A " The date time of modified date of this attribute  
   permissions " id_perms" list(dict) "No " CRU " generated " N/A " The owner and access level
   group " permissions" string "No " CRU " generated " N/A " The group of this attribute
   group_access " permissions" int "No " CRU " generated " 0-7 " The access type of group 
   other_access " permissions" int "No " CRU " generated " 0-7 " The access type of others
   owner " permissions" string "No " CRU " generated " N/A  " The name of the ownter of this attribute
   owner_access " permissions" int "No " CRU " generated " 0-7 " The access type of the ownter
   user_visible " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is visible by user or not 
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid" int "No " R " generated " N/A " For internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   name " routing-instance" string "No " CRU " generated " N/A " The name of thie attribute  
   parent_href " routing-instance" string "No " R " generated " N/A " The URI of this attribute
   parent_type " routing-instance" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " routing-instance" uuid-str "No " R " generated " N/A " The UUID of this attribute
   route_target_refs " routing-instance" list(str)" No " CR "N/A " N/A " The root of this attribute
   attr " route_target_refs" N/A "No " CR "N/A " N/A " The root of this attribute
   import_export " attr" string "N/A " CRUD " null" N/A  " The import_export value 
   href " route_target_refs" string "No " R " generated " N/A " The URI of the interface  
   to " route_target_refs"  list(str) "Yes " CRD " [] "  Valid IPAM form <name>  " The list of this attribute 
   uuid " route_target_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute    
   routing_instance_refs " routing-instance" list(str)"No " CR "N/A " N/A " The root of this attribute 
   attr " routing_instance_refs" N/A "No " CR "N/A " N/A " The root of this attribute  
   href " routing_instance_refs" string "No " R " generated " N/A " The URI of the interface
   to " routing_instance_refs" list(str) "Yes " CRD " [] "  Valid IPAM form <domain>,<project>,<network>,<name>  " The list of this attribute
   uuid " routing_instance_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   uuid " routing-instance" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   virtual_machine_interface_back_refs " list(str)"  N/A "No " R "generated " N/A " The root of this attribute   
   attr " virtual_machine_interface_back_refs" N/A "No " R "generated " N/A " The root of this attribute 
   direction " attr" string "No " R "generated " {ingress|egress|both} " The direction type 
   dst_mac " attr" string "No " R " null " Valid MAC address " The destination MAC address
   mpls_label " attr" integer "No " R " Null " N/A " The MPLS label value
   protocol " attr" string "No " R " Null " {tcp|udp|icmp|any} " The protocol type 
   service_chain_address "attr" string "No " R " Null " Valid IP address" The service chain address
   src_mac " attr" string "No " R " null " Valid MAC address " The source MAC address
   vlan_tag " attr" integer "No " R " null " Valid MAC address " The VLAN ID
   href " virtual_machine_interface_back_refs"  string "No " R " null " Valid MAC address " The destination MAC address 
   to " virtual_machine_interface_back_refs" ist(str) "Yes " R " [] "  Valid IPAM form <domain>,<project>,<name>  " The list of this attribute
   uuid " virtual_machine_interface_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute

routing-instances JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "routing-instance": {
           "display_name": "mac1", 
           "fq_name": [
               "default-domain", 
               "admin", 
               "mac1", 
               "mac1"
           ], 
           "href": "http://127.0.0.1:8082/routing-instance/5ab05ed4-7f71-4299-9015-6ab7cda4bd37", 
           "id_perms": {
               "created": "2015-01-21T10:06:43.187113", 
               "description": null, 
               "enable": true, 
               "last_modified": "2015-01-23T08:53:07.332113", 
               "permissions": {
                   "group": "admin", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 10382321853634231607, 
                   "uuid_mslong": 6534827326078796441
               }
           }, 
           "name": "mac1", 
           "parent_href": "http://127.0.0.1:8082/virtual-network/a8d51c18-b4f8-4309-a28f-d185a39c86c2", 
           "parent_type": "virtual-network", 
           "parent_uuid": "a8d51c18-b4f8-4309-a28f-d185a39c86c2", 
           "route_target_refs": [
               {
                   "attr": {
                       "import_export": null
                   }, 
                   "href": "http://127.0.0.1:8082/route-target/01292b81-0871-4e7b-ac7e-20be894128fa", 
                   "to": [
                       "target:64512:8000006"
                   ], 
                   "uuid": "01292b81-0871-4e7b-ac7e-20be894128fa"
               } 
           ], 
           "routing_instance_refs": [
               {
                   "attr": {}, 
                   "href": "http://127.0.0.1:8082/routing-instance/9c26f0de-846a-40b9-a394-3103bcc1a786", 
                   "to": [
                       "default-domain", 
                       "admin", 
                       "mac2", 
                       "mac2"
                   ], 
                   "uuid": "9c26f0de-846a-40b9-a394-3103bcc1a786"
               }
           ], 
           "uuid": "5ab05ed4-7f71-4299-9015-6ab7cda4bd37", 
           "virtual_machine_interface_back_refs": [
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
                   "href": "http://127.0.0.1:8082/virtual-machine-interface/1ae35391-f7c3-4b80-9fdc-9963e6568c02", 
                   "to": [
                       "default-domain", 
                       "admin", 
                       "1ae35391-f7c3-4b80-9fdc-9963e6568c02"
                   ], 
                   "uuid": "1ae35391-f7c3-4b80-9fdc-9963e6568c02"
               } 
           ]
       }
   }
