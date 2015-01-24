====================
global-system-config
====================

 global-system-configs includes global configuration, belonged vrouter, physical router and so on 

global-system-configs Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   autonomous_system " global-system-config" integer "Yes " CRU " null " N/A " The autonomus system number of this Contrail
   config_version " global-system-config" N/A "No " R " N/A " N/A " The version of this Contrail
   fq_name " global-system-config" list(str) "Yes " CR " null " Valid form <name> " The full query name of this attribute
   global_vrouter_configs " global-system-config" N/A "No " N/A " [] " N/A " The root of this attribute
   href " global_vrouter_configs" string "No " R " generated " N/A " The URI of this attribute
   to " global_vrouter_configs" list(str) "No " CR " [] " Valid form <system-config>,<vrouter-config>" The list of this attribute
   uuid " global_vrouter_configs" uuid-str "No " R " generated " N/A " The UUID of this attribute
   href " global-system-config" string "No " R " generated " N/A " The URI of this attribute
   id_perms " virtual-network" N/A "No " CR "generated " N/A " The root of this attribute
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
   name " global-system-config" string "No " CRU " generated " N/A " The name of thie attribute 
   physical_routers " global-system-config" N/A "No "CR" [] " N/A " The root of this attribute
   href " physical_routers" string "No " R " genereted " N/A " The URI of this attribute
   to " physical_routers" list(str) "No " CR " [] " Valid form <system-config>,<name>" The list of this attribute     
   uuid " physical_routers" string "No " R " generated " N/A " The URI of this attribute
   uuid " global-system-config" string "No " R " generated  "N/A" The URI of this attribute
   virtual_routers " global-system-config" N/A "No " N/A " [] " N/A " The root of this attribute
   to " virtual_routers" list(str) "No " CR " [] " Valid form <system-config>,<name> " The list of this attribute     
   href " virtual_routers" string "No " R " genereted " N/A " The URI of this attribute
   uuid " virtual_routers" string "No " R " generated " N/A "The URI of this attribute

global-system-configs JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "global-system-config": {
           "autonomous_system": <AS_NUMBER>, 
           "config_version": "1.0", 
           "fq_name": [
               "<NAME>"
           ], 
           "global_vrouter_configs": [
               {
                   "href": "http://<API-SERVER>/global-vrouter-config/<UUID>", 
                   "to": [
                       "<NAME>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "href": "http://<API-SERVER>/global-system-config/<UUID>", 
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
                   "uuid_lslong": 13636521902254552987, 
                   "uuid_mslong": 17179920226420736978
               }
           }, 
           "name": "<NAME>", 
           "physical_routers": [
               {
                   "href": "http://<API-SERVER>/physical-router/<UUID>", 
                   "to": [
                       "<NAME>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "uuid": "<UUID>", 
           "virtual_routers": [
               {
                   "href": "http://<API-SERVER>/virtual-router/<UUID>", 
                   "to": [
                       "<NAME>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }, 
           ]
       }
   }
