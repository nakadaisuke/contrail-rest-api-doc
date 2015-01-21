====================
logical-interface
====================

 Put here  description of attribute 

logical-interfaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   logical_interface_vlan_tag " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_refs " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_machine_interface_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_machine_interface_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_interface_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_machine_interface_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   logical_interface_type " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
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
   name " logical-interface" Type "Requ " CRU " Default " Valid " ABCDE
logical-interfaces JSON
====

.. highlight:: json
   :linenothreshold: 5

::