====================
floating-ip
====================

 floating-ip includes IP address of Floating-ip,belonging project,virtual machine interface and so on 

floating-ips Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " floating-ip" string "No " CR " generated " N/A " Display name 
   floating_ip_address " floating-ip" string "Yes " CRU " null " Valid IP address " The Floating IP address
   fq_name " floating-ip" list(str) "Yes " CR " N/A " Valid form <domain>,<project>,<network>,<attribute>,<name>" The full query name of this attribute
   href " floating-ip" string "No " R " generated " N/A " The URI of this attribute
   id_perms " floating-ip" N/A "No " CR "generated " N/A " The root of this attribute
   created " id_perms" datetime "No " R " generated " N/A " The date time of created date of this attribute 
   description " id_perms" string "No " CRU " null " N/A " Description of this attribute
   enable " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is enable or not 
   last_modified " id_perms" datetime "No " R " generated " N/A " The date time of modified date of this attribute  
   permissions " id_perms" list(dict) "No " CRU " generated " N/A " The owner and access level
   group " permissions" string "No " CRU " generated " N/A " The group of this attribute
   group_access " permissions" int "No " CRU " generated " 0-7 " Access type of group 
   other_access " permissions" int "No " CRU " generated " 0-7 " Access type of others
   owner " permissions" string "No " CRU " generated " N/A  " The name of the ownter of this attribute
   owner_access " permissions" int "No " CRU " generated " 0-7 " Access type of the ownter
   user_visible " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is visible by user or not 
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid" int "No " R " generated " N/A " for internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   name " floating-ip" string "No " CRU " generated " N/A " The name of thie attribute 
   parent_href " floating-ip" string "No " R " generated " N/A " The URI of this attribute
   parent_type " floating-ip" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " floating-ip" uuid-str "No " R " generated " N/A " The UUID of this attribute
   project_refs " floating-ip" N/A "No " CR " N/A " N/A " The root of this attribute
   attr " project_refs" string "No " CRU " null " N/A " The attribute of this list
   href " project_refs" string "No " R " generated " N/A " The URI of this attribute  
   to " project_refs" string "No " R " [] " Valid form <domain>,<project> " The attribute of this list 
   uuid " project_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid " floating-ip" uuid-str "No " R " generated " N/A " The UUID of this attribute
   virtual_machine_interface_refs " floating-ip" N/A "No " CR " N/A " N/A " The root of this attribute    
   attr " virtual_machine_interface_refs" string "No " CRU " null " N/A " The attribute of this list 
   href " virtual_machine_interface_refs" string "No " R " generated " N/A " The URI of this attribute  
   to " virtual_machine_interface_refs" string "No " R " [] " Valid form <domain>,<project>,<port> " The attribute of this list  
   uuid " virtual_machine_interface_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute

floating-ips JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "floating-ip": {
           "display_name": "<UUID>", 
           "floating_ip_address": "<IP_ADDRESS>", 
           "fq_name": [
               "<DOMAIN>", 
               "<PROJECT>", 
               "<NETWORK>", 
               "<ATTRIBUTE>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/floating-ip/<UUID>", 
           "id_perms": {
               "created": "<DATE>", 
               "description": null, 
               "enable": true, 
               "last_modified": "<DATE>", 
               "permissions": {
                   "group": "admin", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 12877206164474372262, 
                   "uuid_mslong": 10979627724727797330
               }
           }, 
           "name": "<UUID>", 
           "parent_href": "http://<API-SERVER>/floating-ip-pool/<UUID>", 
           "parent_type": "floating-ip-pool", 
           "parent_uuid": "<UUID>", 
           "project_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/project/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "uuid": "<UUID>", 
           "virtual_machine_interface_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/virtual-machine-interface/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<PORT-NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ]
       }
   }
