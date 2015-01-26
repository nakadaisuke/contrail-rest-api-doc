====================
virtual-DNS
====================

 Put here  description of attribute

virtual-DNSs Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " virtual-DNS" string "No " CR " generated " N/A " The display name
   fq_name " virtual-DNS" list(str) "Yes " CR " [] " Valid form <domain>,<name>" The full query name of this attribute
   href " virtual-DNS" string "No " R " generated " N/A " The URI of this attribute
   id_perms " virtual-DNS" N/A "No " CRU "N/A " N/A " The root of this attribute
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
   name " virtual-DNS" string "No " CRU " generated " N/A " The name of thie attribute
   network_ipam_back_refs " virtual-DNS" list(str) "No " R " generated " N/A " The root of this attribute
   attr " network_ipam_back_refs" string "No " R " generated " N/A " The root of this attribute
   sequence " attr" string "No " R " generated " N/A " The root of this attribute
   major " sequence" integer "No " R " N/A " N/A " The major sequence
   minor " sequence" integer "No " R " N/A " N/A " The minor sequence
   href " network_ipam_back_refs"string "No " R " generated " N/A " The URI of this attribute
   to " network_ipam_back_refs" list(str) "No " R " [] " Valid form <domain>,<project>,<ipam> " The list of this attribute
   uuid " network_ipam_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute
   parent_href " virtual-DNS" string "No " R " generated " N/A " The URI of this attribute
   parent_type " virtual-DNS" string "Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " virtual-DNS" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid " virtual-DNS" uuid-str "No " R " generated " N/A " The UUID of this attribute
   virtual_DNS_data " virtual-DNS" string "No " CR " generated " N/A " The root of this attribute
   default_ttl_seconds " virtual_DNS_data" integer "No " CRU " N/A " N/A " The default TTL seconds
   domain_name " virtual_DNS_data" string "N/A " CRU " N/A " N/A " The domain name
   dynamic_records_from_client " virtual_DNS_data"bool "No " CRU " null "Valid form {true|false} " Specifies whethere dynamic record is enable or not
   floating_ip_record " virtual_DNS_data" string "No " CRU " null " Varid form {dashed-ip|dashed-ip-tenant-name|vm-name|vm-name-tenant-name} " The floating IP recored
   next_virtual_DNS " virtual_DNS_data" string "No " CRUD " null " N/A " The next virtual DNS
   record_order " virtual_DNS_data" string "No " CRU " null " Valid form {fixed|random|round-robin}" The record order
   virtual_DNS_records " virtual-DNS" list(str) "No " CRUD "N/A " N/A " The root of this attribute
   href " virtual_DNS_records" string "No " R " generated " N/A " The URI of this attribute
   to " virtual_DNS_records" list(str) "No " CRD " [] " Valid form <domain>,<dns>,<record> " The list of this attribute
   uuid " virtual_DNS_records" uuid-str "No " R " generated " N/A " The UUID of this attribute

virtual-DNSs JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-DNS": {
           "display_name": "<NAME>",
           "fq_name": [
               "<DOMAIN>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/virtual-DNS/<UUID>",
           "id_perms": {
               "created": "<DATE>",
               "description": null,
               "enable": true,
               "last_modified": "<DATE>",
               "permissions": {
                   "group": "<GROUP>",
                   "group_access": 7,
                   "other_access": 7,
                   "owner": "<OWNTER>",
                   "owner_access": 7
               },
               "user_visible": true,
               "uuid": {
                   "uuid_lslong": 13604631018762302276,
                   "uuid_mslong": 6260782769506697271
               }
           },
           "name": "<NAME>",
           "network_ipam_back_refs": [
               {
                   "attr": {
                       "sequence": {
                           "major": 0,
                           "minor": 0
                       }
                   },
                   "href": "http://<API-SERVER>/network-ipam/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROJECT>",
                       "<IPAM>"
                   ],
                   "uuid": "<UUID>"
               }
           ],
           "parent_href": "http://<API-SERVER>/domain/<UUID>",
           "parent_type": "domain",
           "parent_uuid": "<UUID>",
           "uuid": "<UUID>",
           "virtual_DNS_data": {
               "default_ttl_seconds": <TTL>,
               "domain_name": "<NAME>",
               "dynamic_records_from_client": true,
               "floating_ip_record": "<TYPE>",
               "next_virtual_DNS": "<DNS-SERVER>",
               "record_order": "<ORDER>"
           },
           "virtual_DNS_records": [
               {
                   "href": "http://<API-SERVER>/virtual-DNS-record/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<DNS>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               }
           ]
       }
   }

