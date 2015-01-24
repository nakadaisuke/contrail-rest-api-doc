====================
project
====================

 Put here  description of attribute 

projects Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " project" string "No " CR " generated " N/A " The display name 
   floating_ip_back_refs " project" string "No " R " generated " N/A " The attribute of this list 
   attr " floating_ip_back_refs" string "No " R " generated " N/A " The attribute of this list 
   to " floating_ip_back_refs" list(str) "No " R " generated " Valid form <domain>,<project>,<network>,<attribute>,<uuid> " The list of this attribute 
   href " floating_ip_back_refs" string "No " R " generated " N/A " The URI of this attribute 
   uuid " floating_ip_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   fq_name " project "Yes " CR " [] " Valid form <domain>,<name>" The full query name of this attribute 
   href " project" string "No " R " generated " N/A " The URI of this attribute 
   id_perms " project" N/A "No " CRU "N/A " N/A " The root of this attribute
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
   logical_routers " project" string "No " R " generated " N/A " The attribute of this list
   href " logical_routers" string "No " R " generated " N/A " The URI of this attribute 
   to " logical_routers" list(str) "No " R " genereted " Valid form <domain>,<project>,<name> " The list of this attribute 
   uuid " logical_routers" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   name " project" string "No " CRU " generated " N/A " The name of thie attribute  
   network_ipams " project" string "No " R " generated " N/A " The attribute of this list 
   href " network_ipams" string "No " R " generated " N/A " The URI of this attribute
   to " network_ipams" list(str) "No " R " generated " Valid form <domain>,<network>,<name> " The list of this attribute 
   uuid " network_ipams" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   network_policys " project" string "No " R " generated " N/A " The attribute of this list 
   href " network_policys" string "No " R " generated " N/A " The URI of this attribute 
   to " network_policys" list(str) "No " R " generated " Valid form <domain>,<network>,<name> " The list of this attribute 
   uuid " network_policys" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   parent_href " virtual-network" string "No " R " generated " N/A " The URI of this attribute
   parent_type " virtual-network" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " virtual-network" uuid-str "No " R " generated " N/A " The UUID of this attribute
   quota " project" N/A "No " CR " N/A " N/A " The root of this attribute 
   access_control_list " quota" integer "No " CRU " null " N/A " The access control list quota number 
   bgp_router " quota" integer "No " CRU " null " N/A " The bgp router quota number
   defaults " quota" integer "No " CRU " null " N/A " The default quota number
   floating_ip " quota" integer "No " CRU " -1 " N/A " The Floating IP quota number
   floating_ip_pool " quota" integer "No " CRU " null " N/A " The floating IP pool quota number
   global_vrouter_config " quota" integer "No " CRU " null " N/A " The vRouter quota number
   instance_ip " quota" integer "No " CRU " null " N/A " The instance IP quota number
   logical_router " quota" integer "No " CRU " -1 " N/A " The logical router quota number
   network_ipam " quota" integer "No " CRU " null " N/A " The network IPAM quota number
   security_group " quota" integer "No " CRU " -1 " N/A " The security group quota number
   security_group_rule " quota" integer "No " CRU " null " N/A " The security groute rule quota number
   service_instance " quota" integer "No " CRU " null " N/A " The service instance quota number
   service_template " quota" integer "No " CRU " null " N/A " The service template quota number
   subnet " quota" integer "No " CRU " -1 " N/A " The subnet quota number
   virtual_DNS " quota" integer "No " CRU " null " N/A " The virtual DNS quota number
   virtual_DNS_record " quota" integer "No " CRU " null " N/A " The virtual DNS record quota number
   virtual_machine_interface " quota" integer "No " CRU " -1 " N/A " The virtual machine interface quota number
   virtual_network " quota"  integer "No " CRU " -1 " N/A " The virtual network quota number
   virtual_router " quota"  integer "No " CRU " null " N/A " The virtual router quota number
   route_tables " project" string "No " R " generated " N/A " The attribute of this list 
   href " route_tables" string "No " R " generated " N/A " The URI of this attribute 
   to " route_tables" list(str) "No " R " generated " Valid form <domain>,<project>,<name> " The list of this attribute 
   uuid " route_tables" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   security_groups " project" string "No " R " generated " N/A " The attribute of this list 
   href " security_groups" string "No " R " generated " N/A " The URI of this attribute 
   to " security_groups" list(str) "No " R " generated " Valid form <domain>,<project>,<name> " The list of this attribute 
   uuid " security_groups" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   service_instances " project" string "No " R " generated " N/A " The attribute of this list 
   href " service_instances" string "No " R " generated " N/A " The URI of this attribute 
   to " service_instances" list(str) "No " R " generated " Valid form <domain>,<project>,<name> " The list of this attribute 
   uuid " service_instances" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   uuid " project" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   virtual_machine_interfaces " project " string "No " R " generated " N/A " The attribute of this list 
   href " virtual_machine_interfaces" string "No " R " generated " N/A " The URI of this attribute 
   to " virtual_machine_interfaces" list(str) "No " R " generated " Valid form <domain>,<project>,<name> " The list of this attribute 
   uuid " virtual_machine_interfaces" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   virtual_networks " project" string "No " R " generated " N/A " The attribute of this list 
   href " virtual_networks" string "No " R " generated " N/A " The URI of this attribute 
   to " virtual_networks" list(str) "No " R " generated " Valid form <domain>,<project>,<name> " The list of this attribute 
   uuid " virtual_networks" uuid-str "No " R " generated " N/A " The UUID of this attribute 

projects JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "project": {
           "display_name": "<PROJECT>", 
           "floating_ip_back_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/floating-ip/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NETWORK>", 
                       "<ATTRIBUTE>", 
                       "<UUID>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "fq_name": [
               "<DOMAIN>", 
               "<PROJECT>"
           ], 
           "href": "http://<API-SERVER>/project/<UUID>", 
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
                   "uuid_lslong": 9439552104014199478, 
                   "uuid_mslong": 11410895243465736748
               }
           }, 
           "logical_routers": [
               {
                   "href": "http://<API-SERVER>/logical-router/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "testrt"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "name": "<PROJECT>", 
           "network_ipams": [
               {
                   "href": "http://<API-SERVER>/network-ipam/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "network_policys": [
               {
                   "href": "http://<API-SERVER>/network-policy/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               } 
           ], 
           "parent_href": "http://<API-SERVER>/domain/<UUID>", 
           "parent_type": "domain", 
           "parent_uuid": "<UUID>", 
           "quota": {
               "access_control_list": null, 
               "bgp_router": null, 
               "defaults": null, 
               "floating_ip": -1, 
               "floating_ip_pool": null, 
               "global_vrouter_config": null, 
               "instance_ip": null, 
               "logical_router": -1, 
               "network_ipam": null, 
               "security_group": -1, 
               "security_group_rule": -1, 
               "service_instance": null, 
               "service_template": null, 
               "subnet": -1, 
               "virtual_DNS": null, 
               "virtual_DNS_record": null, 
               "virtual_machine_interface": -1, 
               "virtual_network": -1, 
               "virtual_router": null
           }, 
           "route_tables": [
               {
                   "href": "http://<API-SERVER>/route-table/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "security_groups": [
               {
                   "href": "http://<API-SERVER>/security-group/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "service_instances": [
               {
                   "href": "http://<API-SERVER>/service-instance/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "uuid": "<UUID>", 
           "virtual_machine_interfaces": [
               {
                   "href": "http://<API-SERVER>/virtual-machine-interface/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               } 
           ], 
           "virtual_networks": [
               {
                   "href": "http://<API-SERVER>/virtual-network/<UUID>", 
                   "to": [
                       ":<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ]
       }
   }
