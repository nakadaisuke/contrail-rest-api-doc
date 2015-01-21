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
   parent_uuid " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
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
   display_name " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
   name " virtual-DNS" Type "Requ " CRU " Default " Valid " ABCDE
virtual-DNSs JSON
====

.. highlight:: json
   :linenothreshold: 5

::