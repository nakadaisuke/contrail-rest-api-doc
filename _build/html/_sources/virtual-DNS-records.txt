====================
virtual-DNS-record
====================

 Put here  description of attribute 

virtual-DNS-records Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " virtual-DNS-record" string "No " CR " generated " N/A " The display name 
   fq_name " virtual-DNS-record" list(str) "Yes " CR " [] " Valid form <domain>,<dns>,<name>" The full query name of this attribute 
   href " virtual-DNS-record" string "No " R " generated " N/A " The URI of this attribute 
   id_perms " virtual-DNS-record" N/A "No " CRU "N/A " N/A " The root of this attribute
   created " id_perms" datetime "No " R " generated " N/A " The date time of created date of this attribute 
   description " id_perms" string "No " CRU " null " N/A " The description of this attribute
   enable " id_perms" bool "No " CRU " true "Valid form {true|false} " Specifies whethere this attribute is enable or not 
   last_modified " id_perms" datetime "No " R " generated " N/A " The date time of modified date of this attribute  
   permissions " id_perms" list(dict) "No " CRU " generated " N/A " The owner and access level
   group " permissions" string "No " CRU " generated " N/A " The group of this attribute
   group_access " permissions" int "No " CRU " generated " 0-7 " The access type of group 
   other_access " permissions" int "No " CRU " generated " 0-7 " The access type of others
   owner " permissions" string "No " CRU " generated " N/A  " The name of the ownter of this attribute
   owner_access " permissions" int "No " CRU " generated " 0-7 " The access type of the ownter
   user_visible " id_perms" bool "No " CRU " true "Valid form {true|false} " Specifies whethere this attribute is visible by user or not 
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid" int "No " R " generated " N/A " For internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   name " virtual-DNS-record" string "No " CRU " generated " N/A " The name of thie attribute  
   parent_href " virtual-network" string "No " R " generated " N/A " The URI of this attribute
   parent_type " virtual-network" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " virtual-network" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute  
   virtual_DNS_record_data " virtual-DNS-record" N/A "No " CR " N/A " N/A " The root of this attribute 
   record_class " virtual_DNS_record_data" string "Yes " CRU " null "Valid form  {IN} " The record class
   record_data " virtual_DNS_record_data" string "Yes " CRU " null " N/A " The record data
   record_name " virtual_DNS_record_data" string "Yes " CRU " null " N/A " The record name
   record_ttl_seconds " virtual_DNS_record_data" integer "Yes " CRU " null " N/A " The record TTL
   record_type " virtual_DNS_record_data" string "Yes " CRU " null "Valid form  {A|AAAA|CNAME|PTR|NS} " The record class 

virtual-DNS-records JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-DNS-record": {
           "display_name": "<NAME>", 
           "fq_name": [
               "<DOMAIN>", 
               "<DNS>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/virtual-DNS-record/<UUID>", 
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
                   "uuid_lslong": 11151651069801405736, 
                   "uuid_mslong": 7489262023911294091
               }
           }, 
           "name": "<NAME>", 
           "parent_href": "http://<API-SERVER>/virtual-DNS/<UUID>", 
           "parent_type": "virtual-DNS", 
           "parent_uuid": "<UUID>", 
           "uuid": "<UUID>", 
           "virtual_DNS_record_data": {
               "record_class": "<CLASS>", 
               "record_data": "<DATA>", 
               "record_name": "<NAME>", 
               "record_ttl_seconds": <TTL>, 
               "record_type": "<TYPE>"
           }
       }
   }

