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

   fq_name " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_DNS_record_data " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   record_type " virtual_DNS_record_data" Type "Requ " CRU " Default " Valid " ABCDE
   record_ttl_seconds " virtual_DNS_record_data" Type "Requ " CRU " Default " Valid " ABCDE
   record_name " virtual_DNS_record_data" Type "Requ " CRU " Default " Valid " ABCDE
   record_class " virtual_DNS_record_data" Type "Requ " CRU " Default " Valid " ABCDE
   record_data " virtual_DNS_record_data" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
   name " virtual-DNS-record" Type "Requ " CRU " Default " Valid " ABCDE
virtual-DNS-records JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-DNS-record": {
           "display_name": "67ef3421-850e-448b-9ac2-9f90629e1d28", 
           "fq_name": [
               "default-domain", 
               "dns1", 
               "67ef3421-850e-448b-9ac2-9f90629e1d28"
           ], 
           "href": "http://127.0.0.1:8082/virtual-DNS-record/67ef3421-850e-448b-9ac2-9f90629e1d28", 
           "id_perms": {
               "created": "2014-12-09T23:23:09.323434", 
               "description": null, 
               "enable": true, 
               "last_modified": "2014-12-09T23:23:09.323434", 
               "permissions": {
                   "group": "admin", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 11151651069801405736, 
                   "uuid_mslong": 7489262023911294091
               }
           }, 
           "name": "67ef3421-850e-448b-9ac2-9f90629e1d28", 
           "parent_href": "http://127.0.0.1:8082/virtual-DNS/56e2c4c2-0055-4037-bccd-5bd4c5967344", 
           "parent_type": "virtual-DNS", 
           "parent_uuid": "56e2c4c2-0055-4037-bccd-5bd4c5967344", 
           "uuid": "67ef3421-850e-448b-9ac2-9f90629e1d28", 
           "virtual_DNS_record_data": {
               "record_class": "IN", 
               "record_data": "10.0.0.1", 
               "record_name": "testhost1", 
               "record_ttl_seconds": 86400, 
               "record_type": "A"
           }
       }
   }

