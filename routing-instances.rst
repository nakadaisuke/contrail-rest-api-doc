====================
routing-instance
====================

 Put here  description of attribute 

routing-instances Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   parent_href " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   fq_name " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_back_refs " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   dst_mac " attr" Type "Requ " CRU " Default " Valid " ABCDE
   protocol " attr" Type "Requ " CRU " Default " Valid " ABCDE
   direction " attr" Type "Requ " CRU " Default " Valid " ABCDE
   mpls_label " attr" Type "Requ " CRU " Default " Valid " ABCDE
   vlan_tag " attr" Type "Requ " CRU " Default " Valid " ABCDE
   src_mac " attr" Type "Requ " CRU " Default " Valid " ABCDE
   service_chain_address " attr" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   href " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   route_target_refs " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   to " route_target_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " route_target_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " route_target_refs" Type "Requ " CRU " Default " Valid " ABCDE
   import_export " attr" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " route_target_refs" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
   name " routing-instance" Type "Requ " CRU " Default " Valid " ABCDE
routing-instances JSON
====

.. highlight:: json
   :linenothreshold: 5

::