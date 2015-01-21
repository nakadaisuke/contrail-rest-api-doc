====================
global-vrouter-config
====================

 Put here  description of attribute 

global-vrouter-configs Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   linklocal_services " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   linklocal_service_entry " linklocal_services" Type "Requ " CRU " Default " Valid " ABCDE
   linklocal_service_name " linklocal_service_entry" Type "Requ " CRU " Default " Valid " ABCDE
   ip_fabric_service_ip " linklocal_service_entry" Type "Requ " CRU " Default " Valid " ABCDE
   linklocal_service_ip " linklocal_service_entry" Type "Requ " CRU " Default " Valid " ABCDE
   ip_fabric_service_port " linklocal_service_entry" Type "Requ " CRU " Default " Valid " ABCDE
   ip_fabric_DNS_service_name " linklocal_service_entry" Type "Requ " CRU " Default " Valid " ABCDE
   linklocal_service_port " linklocal_service_entry" Type "Requ " CRU " Default " Valid " ABCDE
   encapsulation_priorities " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   encapsulation " encapsulation_priorities" Type "Requ " CRU " Default " Valid " ABCDE
   href " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
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
   fq_name " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   vxlan_network_identifier_mode " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
   name " global-vrouter-config" Type "Requ " CRU " Default " Valid " ABCDE
global-vrouter-configs JSON
====

.. highlight:: json
   :linenothreshold: 5

::