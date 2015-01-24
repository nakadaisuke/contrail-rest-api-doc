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

   fq_name " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_DNS_records " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_DNS_records" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_DNS_records" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_DNS_records" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   name " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   network_ipam_back_refs " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   to " network_ipam_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " network_ipam_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " network_ipam_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " network_ipam_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_DNS_data " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   floating_ip_record " virtual_DNS_data" Type "Requ " CRU " Default " Valid " ABCDE
   domain_name " virtual_DNS_data" Type "Requ " CRU " Default " Valid " ABCDE
   next_virtual_DNS " virtual_DNS_data" Type "Requ " CRU " Default " Valid " ABCDE
   dynamic_records_from_client " virtual_DNS_data" Type "Requ " CRU " Default " Valid " ABCDE
   default_ttl_seconds " virtual_DNS_data" Type "Requ " CRU " Default " Valid " ABCDE
   record_order " virtual_DNS_data" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE


virtual-DNSs JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-DNS": {
           "display_name": "dns1", 
           "fq_name": [
               "default-domain", 
               "dns1"
           ], 
           "href": "http://127.0.0.1:8082/virtual-DNS/56e2c4c2-0055-4037-bccd-5bd4c5967344", 
           "id_perms": {
               "created": "2014-12-09T21:41:58.578435", 
               "description": null, 
               "enable": true, 
               "last_modified": "2014-12-09T21:41:58.578435", 
               "permissions": {
                   "group": "admin", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 13604631018762302276, 
                   "uuid_mslong": 6260782769506697271
               }
           }, 
           "name": "dns1", 
           "network_ipam_back_refs": [
               {
                   "attr": null, 
                   "href": "http://127.0.0.1:8082/network-ipam/460728e1-9bf5-47f5-8504-c21605562ba1", 
                   "to": [
                       "default-domain", 
                       "admin", 
                       "ssssss"
                   ], 
                   "uuid": "460728e1-9bf5-47f5-8504-c21605562ba1"
               }, 
               {
                   "attr": {
                       "sequence": {
                           "major": 0, 
                           "minor": 0
                       }
                   }, 
                   "href": "http://127.0.0.1:8082/network-ipam/b81f0b37-8304-42ea-94a0-c15be022c5d6", 
                   "to": [
                       "default-domain", 
                       "default-project", 
                       "default-network-ipam"
                   ], 
                   "uuid": "b81f0b37-8304-42ea-94a0-c15be022c5d6"
               }
           ], 
           "parent_href": "http://127.0.0.1:8082/domain/11e2ba75-241a-435c-879d-0dcad6253169", 
           "parent_type": "domain", 
           "parent_uuid": "11e2ba75-241a-435c-879d-0dcad6253169", 
           "uuid": "56e2c4c2-0055-4037-bccd-5bd4c5967344", 
           "virtual_DNS_data": {
               "default_ttl_seconds": 86400, 
               "domain_name": "testdomein1", 
               "dynamic_records_from_client": true, 
               "floating_ip_record": "dashed-ip-tenant-name", 
               "next_virtual_DNS": "8.8.8.8", 
               "record_order": "random"
           }, 
           "virtual_DNS_records": [
               {
                   "href": "http://127.0.0.1:8082/virtual-DNS-record/67ef3421-850e-448b-9ac2-9f90629e1d28", 
                   "to": [
                       "default-domain", 
                       "dns1", 
                       "67ef3421-850e-448b-9ac2-9f90629e1d28"
                   ], 
                   "uuid": "67ef3421-850e-448b-9ac2-9f90629e1d28"
               }
           ]
       }
   }

