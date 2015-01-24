====================
instance-ip
====================

 instance-ip includes virtual machine interface, IP address and so on 

instance-ips Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 


   display_name " instance-ip" string "No " CR " generated " N/A " Display name 
   fq_name " instance-ip" list(str) "Yes " CR " [] " Valid form <name>" The full query name of this attribute
   href " instance-ip" string "No " R " generated " N/A " The URI of this attribute
   id_perms " instance-ip" N/A "No " CR "generated " N/A " The root of this attribute
   created " id_perms" datetime "No " R " generated " N/A " The date time of created date of this attribute 
   description " id_perms" string "No " CRU " null " N/A " Description of this attribute
   enable " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is enable or not 
   last_modified " id_perms" datetime "No " R " generated " N/A " The date time of modified date of this attribute  
   permissions " id_perms" list(dict) "No " CRU " generated " N/A " The owner and access level
   group " permissions" string "No " CRU " generated " N/A " The group of this attribute
   group_access " permissions" int "No " CRU " generated " Valid access range 0-7 " Access type of group 
   other_access " permissions" int "No " CRU " generated " Valid access range 0-7 " Access type of others
   owner " permissions" string "No " CRU " generated " N/A  " The name of the ownter of this attribute
   owner_access " permissions" int "No " CRU " generated " Valid access range 0-7 " Access type of the ownter
   user_visible " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is visible by user or not 
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid" int "No " R " generated " N/A " For internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   instance_ip_address " instance-ip" String "Yes " CR " null " Valid IP address " The instance IP address
   instance_ip_family " instance-ip" String "Tes " CR " null " {v4|v6} " IP address family
   name " instance-ip" string "No " CRU " generated " N/A " The name of thie attribute
   uuid " instance-ip" uuid-str "No " R " generated " N/A " The UUID of this attribute
   virtual_machine_interface_refs " string "N/A " R " generated " N/A  " The root of this attribute
   attr " virtual_machine_interface_refs" string "No " R " null " N/A " The list of this attribute 
   href " virtual_machine_interface_refs" string "No " R " generated " N/A " The URI of this attribute 
   to " virtual_machine_interface_refs" list(str) "No " CR " [] " Valid form <domain>,<project>,<virtual-machine-interface> " The list of this attribute
   uuid " virtual_machine_interface_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   virtual_network_refs " instance-ip" string "N/A " R " generated " N/A  " The root of this attribute
   to " virtual_network_refs" list(str) "No " CR " [] " Valid form <domain>,<project>,<network> " The list of this attribute
   attr " virtual_network_refs" string "No " R " null " N/A " The list of this attribute
   href " virtual_network_refs" string "No " R " generated " N/A " The URI of this attribute 
   uuid " virtual_network_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute
 
instance-ips JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "instance-ip": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/instance-ip/<UUID>", 
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
                   "uuid_lslong": 13416391476237010658, 
                   "uuid_mslong": 11165595147455054059
               }
           }, 
           "instance_ip_address": "<IP_ADDRESS>", 
           "instance_ip_family": "v4", 
           "name": "<UUID>", 
           "uuid": "<UUID>", 
           "virtual_machine_interface_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/virtual-machine-interface/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "virtual_network_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/virtual-network/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ]
       }
   }
