====================
service-template
====================

 Put here  description of attribute 

service-templates Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   href " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   service_template_properties " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   availability_zone_enable " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   interface_type " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   static_route_enable " interface_type" Type "Requ " CRU " Default " Valid " ABCDE
   shared_ip " interface_type" Type "Requ " CRU " Default " Valid " ABCDE
   service_interface_type " interface_type" Type "Requ " CRU " Default " Valid " ABCDE
   image_name " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_mode " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_type " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   flavor " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_scaling " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   ordered_interfaces " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " service-template" Type "Requ " CRU " Default " Valid " ABCDE
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
   name " service-template" Type "Requ " CRU " Default " Valid " ABCDE
service-templates JSON
====

.. highlight:: json
   :linenothreshold: 5

::