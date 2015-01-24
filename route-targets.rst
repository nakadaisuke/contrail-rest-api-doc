====================
route-target
====================

 Put here  description of attribute 

route-targets Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Requi<name>,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " route-target" string "No " CR " generated " N/A " The display name 
   fq_name " route-target" list(str) "Yes " CR " [] " Valid form <name>" The full query name of this attribute 
   href " route-target" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " route-target" N/A "No " CRU "N/A " N/A " The root of this attribute
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
   name " route-target" string "No " CRU " generated " N/A " The name of thie attribute 
   routing_instance_back_refs " route-target" string "N/A " R " generated" N/A  " The root of this attribute 
   attr " routing_instance_back_refs" N/A "N/A " R " generated" N/A  " The root of this attribute
   import_export " attr" string "N/A " R " generated" N/A  " The import_export value
   href " routing_instance_back_refs" string "No " R " generated " N/A " The URI of the interface 
   to " routing_instance_back_refs" list(str) "No " R " generated " N/A " The list of this attribute 
   uuid " routing_instance_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   uuid " route-target" uuid-str "No " R " generated " N/A " The UUID of this attribute
 
route-targets JSON
====

.. highlight:: json
   :linenothreshold: 5

::


   {
       "route-target": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/route-target/<UUID>", 
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
                   "uuid_lslong": 9498707767445596670, 
                   "uuid_mslong": 13805884946253627875
               }
           }, 
           "name": "<NAME>", 
           "routing_instance_back_refs": [
               {
                   "attr": {
                       "import_export": null
                   }, 
                   "href": "http://<API-SERVER>/routing-instance/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<PROJECT>", 
                       "<name>", 
                       "<name>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "uuid": "<UUID>"
       }
   }
