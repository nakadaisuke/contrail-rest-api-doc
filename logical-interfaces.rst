====================
logical-interface
====================

 logical-interface includes logical-interface, virtual machine interface and so on 

logical-interfaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " logical-interface" string "No " CR " generated " N/A " Display name
   fq_name " logical-interface"  list(str) "Yes " CR " N/A " Valid form <system-config>,<physical-router>,<physical-interface>,<name>" The full query name of this attribute
   href " logical-interface" string "No " R " generated " N/A " The URI of this attribute
   id_perms " logical-interface" N/A "No " CR "generated " N/A " The root of this attribute
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
   uuid_lslong " uuid" int "No " R " generated " N/A " For internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   logical_interface_type " logical-interface" string "Yes " CRU " N/A " {l2|l3} " The logical interface type
   logical_interface_vlan_tag " logical-interface" integer "Yes " CRU " N/A " 0-4095 " The logical interface VLAN tag ID
   name " logical-interface" string "No " CRU " generated " N/A " The name of thie attribute 
   parent_href " logical-interface" string "No " R " generated " N/A " The URI of this attribute
   parent_type " logical-interface" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " logical-interface" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid " logical-interface" N/A "No " CR " N/A " N/A " The root of this attribute 
   virtual_machine_interface_refs " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_interface_refs" string "No " CRU " null " N/A " The attribute of this list 
   href " virtual_machine_interface_refs" string "No " R " generated " N/A " The URI of this attribute  
   to " virtual_machine_interface_refs" string "No " R " [] " Valid form <domain>,<project>,<port> " The attribute of this list  
   uuid " virtual_machine_interface_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute

logical-interfaces JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "logical-interface": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<SYSTEM-CONFIG>", 
               "<PHYSICAL-ROUTER>", 
               "<PHYSICAL-INTERFACE>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/logical-interface/<UUID>", 
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
                   "uuid_lslong": 10676200096649138542, 
                   "uuid_mslong": 1248102854688591220
               }
           }, 
           "logical_interface_type": <TYPE>, 
           "logical_interface_vlan_tag": <TAG>, 
           "name": "<NAME>", 
           "parent_href": "http://<API-SERVER>/physical-interface/<UUID>", 
           "parent_type": "physical-interface", 
           "parent_uuid": "<UUID>", 
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
           ]
       }
   }
