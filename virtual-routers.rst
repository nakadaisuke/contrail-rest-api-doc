====================
virtual-router
====================

 Put here  description of attribute 

virtual-routers Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " virtual-router" string "No " CR " generated " N/A " The display name  
   fq_name " virtual-router" list(str) "Yes " CR " [] " Valid form <system-config>,<name>" The full query name of this attribute 
   href " virtual-router" string "No " R " generated " N/A " The URI of the interface
   id_perms " virtual-router" N/A "No " CRU "N/A " N/A " The root of this attribute
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
   name " virtual-router" string "No " CRU " generated " N/A " The name of thie attribute   
   parent_href " routing-instance" string "No " R " generated " N/A " The URI of this attribute
   parent_type " routing-instance" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " routing-instance" uuid-str "No " R " generated " N/A " The UUID of this attribute
   physical_router_back_refs " virtual-router" list(str) "No " R "generated " N/A " The root of this attribute 
   attr " physical_router_back_refs" N/A "No " R "generated " N/A " The root of this attribute 
   href " physical_router_back_refs" string "No " R " generated " N/A " The URI of the interface    
   to " physical_router_back_refs" list(str) "No " R " [] "  Valid form <system-config>,<pyhsical-router>  " The list of this attribute 
   uuid " physical_router_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute   
   uuid " virtual-router" uuid-str "No " R " generated " N/A " The UUID of this attribute  
   virtual_machine_refs " virtual-router" list(str)" No " CR "N/A " N/A " The root of this attribute 
   attr " virtual_machine_refs" N/A "No " CR "N/A " N/A " The root of this attribute 
   href " virtual_machine_refs" string "No " R " generated " N/A " The URI of the interface 
   to " virtual_machine_refs"  list(str) "Yes " CRD " [] "  Valid form <name>  " The list of this attribute 
   uuid " virtual_machine_refs"uuid-str "No " R " generated " N/A " The UUID of this attribute   
   virtual_router_ip_address " virtual-router" string "No " CRUD " null " N/A " The virtual router IP address
   virtual_router_type " virtual-router" list(str) "No " CRUD " null " Valid form {embedded|tor-agent|tor-service-node} " The virtual router type 

virtual-routers JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-router": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<SYSTEM-CONFIG>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/virtual-router/<UUID>", 
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
                   "uuid_lslong": 9695899840403396944, 
                   "uuid_mslong": 3325289362864754628
               }
           }, 
           "name": "<NAME>", 
           "parent_href": "http://<API-SERVER>/global-system-config/<UUID>", 
           "parent_type": "global-system-config", 
           "parent_uuid": "<UUID>", 
           "physical_router_back_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/physical-router/<UUID>", 
                   "to": [
                       "<SYSTEM-CONFIG>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "uuid": "<UUID>", 
           "virtual_machine_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/virtual-machine/<UUID>", 
                   "to": [
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "virtual_router_ip_address": "<IP_ADDRESS>", 
           "virtual_router_type": [
               "<TYPE>"
           ]
       }
   }

