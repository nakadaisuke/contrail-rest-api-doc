====================
global-vrouter-config
====================

 global-vrouter-config includes vrouter global configuration, IP fablic service and so on 

global-vrouter-configs Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " global-vrouter-config" string "No " CR " generated " N/A " Display name 
   encapsulation_priorities " global-vrouter-config" N/A "No " CR "generated " N/A " The root of this attribute
   encapsulation " encapsulation_priorities" list(str) "Yes " CRUD " [] " {VXLAN|MPLSoUDP|MPLSoGRE} " The encapsulation protocol type
   fq_name " global-vrouter-config" list(str) "Yes " CR " [] " Valid form <system-config>,<name>" The full query name of this attribute
   href " global-vrouter-config" string "No " R " generated " N/A " The URI of this attribute
   id_perms " global-vrouter-config" N/A "No " CR "generated " N/A " The root of this attribute
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
   linklocal_services " global-vrouter-config" N/A "No " CR " generated " N/A " The root of this attribute
   linklocal_service_entry " linklocal_services" N/A "No " CR " generated " N/A " The root of this attribute
   ip_fabric_DNS_service_name " linklocal_service_entry" string "No " CRU " null " DNS service name " The IP fabfic DNS service name
   ip_fabric_service_ip " linklocal_service_entry" list(str) "No " CRUD " [] " Valid IP address " The list of IP fablic service IP
   ip_fabric_service_port " linklocal_service_entry" integer "No " CRU " N/A " 0-65535 " The linklocal service port
   linklocal_service_ip " linklocal_service_entry" string "No " CRU " null " Valid IP address " The linklocal service IP
   linklocal_service_name " linklocal_service_entry" string "No " CR " N/A " N/A " The linklocal service name
   linklocal_service_port " linklocal_service_entry" integer "No " CRU " N/A " 0-65535 " The linklocal server port
   name " global-vrouter-config"  string "No " CRU " generated " N/A " The name of thie attribute 
   parent_href " global-vrouter-config" string "No " R " generated " N/A " The URI of this attribute 
   parent_type " global-vrouter-config" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " global-vrouter-config" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid " global-vrouter-config"uuid-str "No " R " generated " N/A " The UUID of this attribute
   vxlan_network_identifier_mode " global-vrouter-config" string "Yes " CRU " N/A " {configured|automatic} " The VXLAN network identifier mode 

global-vrouter-configs JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "global-vrouter-config": {
           "display_name": "<NAME>", 
           "encapsulation_priorities": {
               "encapsulation": [
                   "VXLAN", 
                   "MPLSoUDP", 
                   "MPLSoGRE"
               ]
           }, 
           "fq_name": [
               "<SYSTEM_CONFIG>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/global-vrouter-config/<UUID>", 
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
                   "uuid_lslong": 13396100387536944290, 
                   "uuid_mslong": 2550391563090019913
               }
           }, 
           "linklocal_services": {
               "linklocal_service_entry": [
                   {
                       "ip_fabric_DNS_service_name": "", 
                       "ip_fabric_service_ip": [
                           "<IP_ADDRESS>"
                       ], 
                       "ip_fabric_service_port": <PORT>, 
                       "linklocal_service_ip": "<IP_ADDRESS>", 
                       "linklocal_service_name": "<NAME>", 
                       "linklocal_service_port": <PORT>
                   }
               ]
           }, 
           "name": "<NAME>", 
           "parent_href": "http://<API-SERVER>/global-system-config/<UUID>", 
           "parent_type": "global-system-config", 
           "parent_uuid": "<UUID>", 
           "uuid": "<UUID>", 
           "vxlan_network_identifier_mode": "automatic"
       }
   }

