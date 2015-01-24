====================
physical-router
====================

 Put here  description of attribute 

physical-routers Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " physical-router" string "No " CR " generated " N/A " The display name 
   fq_name " physical-router" list(str) "Yes " CR " [] " Valid form <system-config>,<name>" The full query name of this attribute 
   href " physical-router" string "No " R " generated " N/A " The URI of this attribute 
   id_perms " physical-router" N/A "No " CRU "N/A " N/A " The root of this attribute
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
   name " physical-router" string "No " CRU " generated " N/A " The name of thie attribute 
   parent_href " physical-router" string "No " R " generated " N/A " The URI of this attribute
   parent_type " physical-router" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " physical-router" uuid-str "No " R " generated " N/A " The UUID of this attribute
   physical_interfaces " physical-router" list(str) "N/A " CRUD " [] " N/A " The root of this attribute
   href " physical_interfaces" string "No " R " generated " N/A " The URI of this attribute   
   to " physical_interfaces" list(str) "No " CR " [] " Valid form <system-config>,<physical-router><interface> " The list of this attribute 
   uuid " physical_interfaces" uuid-str "No " R " generated " N/A " The UUID of this attribute
   physical_router_dataplane_ip " physical-router" string "No " CRUD " null " Valid IP address" The physical router dataplane IP address
   physical_router_management_ip " physical-router" string "No " CRUD " null " Valid IP address" The physical router management IP address
   physical_router_user_credentials " physical-router" list(dict) "No " CR " N/A " N/A " The root of this attribute
   password " physical_router_user_credentials" string "No " CRUD " null " N/A " The password of this credencials
   username " physical_router_user_credentials" string "No " CRUD " null " N/A " The username of this credencials 
   physical_router_vendor_name " physical-router" string "No " CRUD " null " N/A " The vender name
   uuid " physical_interfaces" uuid-str "No " R " generated " N/A " The UUID of this attribute
   virtual_router_refs " physical-router" list(str) "No " CRUD " [] " N/A " The root of this attribute
   attr " virtual_router_refs" N/A "No " CRUD " null " N/A " The root of this attribute
   href " virtual_router_refs" string "No " R " generated " N/A " The URI of this attribute  
   to " virtual_router_refs" list(str) "No " CR " [] " Valid form <system-config>,<vrouter host> " The list of this attribute 
   uuid " virtual_router_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute 

physical-routers JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "physical-router": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<SYSTEM-CONFIG>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/physical-router/<UUID>", 
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
                   "uuid_lslong": 9475787697541815152, 
                   "uuid_mslong": 8088126446325549993
               }
           }, 
           "name": "<NAME>", 
           "parent_href": "http://<API-SERVER>/global-system-config/<UUID>", 
           "parent_type": "global-system-config", 
           "parent_uuid": "<UUID>", 
           "physical_interfaces": [
               {
                   "href": "http://<API-SERVER>/physical-interface/<UUID>", 
                   "to": [
                       "<SYSTEM-CONFIG>", 
                       "<PHYSICAL-ROUTER>", 
                       "<INTERFACE>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "physical_router_dataplane_ip": "<IP_ADDRESS>", 
           "physical_router_management_ip": "<IP_ADDRESS>", 
           "physical_router_user_credentials": {
               "password": "", 
               "username": ""
           }, 
           "physical_router_vendor_name": "<NAME>", 
           "uuid": "<UUID>", 
           "virtual_router_refs": [
               {
                   "attr": null, 
                   "href": "http://<API-SERVER>/virtual-router/<UUID>", 
                   "to": [
                       "<SYSTEM-CONFIG>", 
                       "<HOST>"
                   ], 
                   "uuid": "<UUID>"
               }
           ]
       }
   }
