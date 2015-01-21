====================
network-ipam
====================

 Put here  description of attribute 

network-ipams Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_network_back_refs " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_network_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_network_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_network_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   ipam_subnets " attr" Type "Requ " CRU " Default " Valid " ABCDE
   host_routes " attr" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_network_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   network_ipam_mgmt " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   ipam_dns_method " network_ipam_mgmt" Type "Requ " CRU " Default " Valid " ABCDE
   ipam_dns_server " network_ipam_mgmt" Type "Requ " CRU " Default " Valid " ABCDE
   tenant_dns_server_address " ipam_dns_server" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_dns_server_name " ipam_dns_server" Type "Requ " CRU " Default " Valid " ABCDE
   href " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
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
   virtual_DNS_refs " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_DNS_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_DNS_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_DNS_refs" Type "Requ " CRU " Default " Valid " ABCDE
   sequence " attr" Type "Requ " CRU " Default " Valid " ABCDE
   major " sequence" Type "Requ " CRU " Default " Valid " ABCDE
   minor " sequence" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_DNS_refs" Type "Requ " CRU " Default " Valid " ABCDE
   name " network-ipam" Type "Requ " CRU " Default " Valid " ABCDE
network-ipams JSON
====

.. highlight:: json
   :linenothreshold: 5

::