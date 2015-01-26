====================
service-template
====================

 Put here  description of attribute 

service-templates Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " service-template" string "No " CR " generated " N/A " The display name 
   fq_name " service-template" list(str) "Yes " CR " [] " Valid form <domain>,<name>" The full query name of this attribute 
   href " service-template" string "No " R " generated " N/A " The URI of this attribute 
   id_perms " service-template" N/A "No " CRU "N/A " N/A " The root of this attribute
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
   name " service-template" string "No " CRU " generated " N/A " The name of thie attribute  
   parent_href " service-template" string "No " R " generated " N/A " The URI of this attribute
   parent_type " service-template" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " service-template" uuid-str "No " R " generated " N/A " The UUID of this attribute
   service_template_properties " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   availability_zone_enable " service_template_properties" bool "No " CRU " false " {true|false} " Specifies whehter the availability zone is enable or not   
   flavor " service_template_properties" string "No " CRU " null " Valid flavor name" The flavor name
   image_name " service_template_properties" string "No " CRU " null " Valid image name" The image name
   interface_type " service_template_properties" list(str) "No " CRUD " [] " N/A " The root of this attribute
   service_interface_type " interface_type" string "No " CRU " null " {management|left|right|other} " The interface type
   static_route_enable " interface_type" bool "No " CRU " false " {true|false} " Specifies whehter the static route is enable or not
   shared_ip " interface_type" bool "No " CRU " false " {true|false} " Specifies whehter the shared IP is enable or not
   ordered_interfaces " service_template_properties" bool "No " CRU " false " {true|false} " Specifies whehter the orderd interface is enable or not   
   service_mode " service_template_properties"string "No " CRU " null " {transparent|in-network|in-network-nat} " The service mode type  
   service_scaling "bool "No " CRU " false " {true|false} " Specifies whehter the service scaling is enable or not  
   service_type " service_template_properties" string "No " CRU " null " {firewall|analyzer|source-nat|loadbalancer} " The service mode type  
   uuid " service-template" uuid-str "No " R " generated " N/A " The UUID of this attribute  

service-templates JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "service-template": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<DOMAIN>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/service-template/<UUID>", 
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
               },s 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 9933517499790756795, 
                   "uuid_mslong": 3722135275090626617
               }
           }, 
           "name": "<NAME>", 
           "parent_href": "http://<API-SERVER>/domain/<UUID>", 
           "parent_type": "domain", 
           "parent_uuid": "<UUID>", 
           "service_template_properties": {
               "availability_zone_enable": true, 
               "flavor": "<FLAVOR>", 
               "image_name": "<IMAGE>", 
               "interface_type": [
                   {
                       "service_interface_type": "<TYPE>", 
                       "shared_ip": true, 
                       "static_route_enable": false
                   }
               ], 
               "ordered_interfaces": true, 
               "service_mode": "<MODE>", 
               "service_scaling": true, 
               "service_type": "<TYPE>"
           }, 
           "uuid": "<UUID>"
       }
   }

