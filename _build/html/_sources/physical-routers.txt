====================
physical-router
====================

 Put here  description of attribute 

physical-routers Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   physical_router_management_ip " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_router_refs " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_router_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_router_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_router_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_router_refs" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   name " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   physical_router_vendor_name " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   href " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   physical_router_user_credentials " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   username " physical_router_user_credentials" Type "Requ " CRU " Default " Valid " ABCDE
   password " physical_router_user_credentials" Type "Requ " CRU " Default " Valid " ABCDE
   fq_name " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   physical_interfaces " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   to " physical_interfaces" Type "Requ " CRU " Default " Valid " ABCDE
   href " physical_interfaces" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " physical_interfaces" Type "Requ " CRU " Default " Valid " ABCDE
   physical_router_dataplane_ip " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " physical-router" Type "Requ " CRU " Default " Valid " ABCDE
physical-routers JSON
====

.. highlight:: json
   :linenothreshold: 5

::